[Read Me.txt](https://github.com/JessJutha/NewHireDataEntry-OnboardingProcess/files/7074094/Read.Me.txt)
# NewHireDataEntry-OnboardingProcess
This is New Hire Data Entry & Onboarding Process feature by Automation 360 x AARI x IQBot

Environment: Oracle HCM Cloud (Fusion) 
ps. Require credential to access not for public release


We learn that one of the challenging processes that the HR team has to face in almost every month is the New hire - Onboarding process. 
It surprisingly involves a lot of teams internally & hard to control the time duration to complete the whole process which may lead to the delay and some miscommunication among the company & the new hire candidates.
This whole process may take around 2 days to complete or even a week without a plan or good upfront communication among the teams who are involved due to the waiting time.
We have analysed the onboarding process and listed down the repetitive, manual tasks that can be handled by bot with the aim to reduce the no. of persons or parties who need to get involved during the process to ultimately reduce the process time overall.

For the overall design, we use AARI to let the bot runner specify the folder to the scanned confirmed employment contract pdf files, then use IQ Bot to scan and prepare the necessary new hire data in CSV. Bot will further use the CSV file to perform the new hire data entry action in the Oracle HCM system and send the summary report back to the HR User when the process ends. After this we allow the bot runner to choose whether to immediately proceed to the onboarding action or not through another AARI screen. If the answer provided is “Yes”, our onboarding bot will kick in and start the onboarding process. During the onboarding, the bot will create new email account, assign related company asset(s) to the employee through the HCM system and send the new hire info. to all related parties like HR Team, Supervisor & New Hire Candidate themselves. 
Via this approach, we can get rid of wait time for the dependable tasks among each Department as bot able to handle 80-90% of the activities, a week lead time process can be done within a few clicks and a lot lesser time like 10-15 min.
 
The challenge that we found:
When bot performs new hire data entry and assign asset/property into HCM system (Oracle HCM Cloud) using Recorder action in Automation 360, we ran into some challenges that bot kept failing whether bot cannot find the element/object in the specific web browser or perform the task too fast even before web browser is fully loaded.
Therefore we added some more Delay action but that cause us some extra minutes until the bot successfully finishes the task. Maybe there's another action or solution to this which we will explore further to improve the effectiveness of this bot and hopefully feature more of AARI capability in the future.

For import Bot, click the link to download : https://drive.google.com/file/d/17r8_C1FCWuvpBagVhFJSlwwerkIlt-K4/view?usp=sharing
