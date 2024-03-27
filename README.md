# Activate-Copilot-in-Windows-11-EU-
Activate Copilot in locked Regions working March 26th

Hello!
  I am one of the few indeviduals who wants copilot access directly from the Windows Taskbar in a locked region.
  to achieve this just follow the stepps below.

Open Microsoft Edge and type 'edge://flags' in the adressbar.
On the page search for 'Allow Bing AI generated workspaces' and enable it.

Click Windows + R to open the RUN Window
type regedit and open it
Once Arrived in the Registry editor go to the placs bellow, if not accessible create it.

HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced\.		
DWord 32bit......... 'ShowCopilotButton' set it to 1
Dword 32bit.........	'Taskbar AI' set it to 1 

Computer\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\WindowsCopilot
Dword 32bit......... 'AllowCopilotRuntime' set to 1

Computer\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\Copilot
Dword 32bit......... 'EnableCopilot' set it to 1

once this is done toggle 'Taskbar AI' or go into the settings and set taskbar to right or middle.
this should "reload" it and copilot should show up.
When not go into the taskbar settings again and looks if copilot is available if not..... then welp idk.
Press Windows + R again and type 'microsoft-edge://?ux=copilot&tcp=1&source=taskbar'
Press enter and copilot should show up, if not, rather a edge window opens, somethings wrong with edge and try step 1 again.
