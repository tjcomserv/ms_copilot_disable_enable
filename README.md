# ms_copilot_disable_enable
Registry file to disable and enable CoPilot in Windows

Just download and run the required reg file.

# Enable
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced]
"EnableCopilot"=dword:00000001
"CopilotEnabledOnStartup"=dword:00000001
"CopilotShowTips"=dword:00000001
"CopilotFeedback"=dword:00000001
"CopilotDataCollection"=dword:00000001

[HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced]
"EnableCopilot"=dword:00000001

[HKEY_CURRENT_USER\Software\Policies\Microsoft\Windows\WindowsCopilot]
"TurnOffWindowsCopilot"=dword:00000000

[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\WindowsCopilot]
"TurnOffWindowsCopilot"=dword:00000000

[HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced]
"TaskbarCopilot"=dword:00000001


# Disable
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced]
"EnableCopilot"=dword:00000000
"CopilotEnabledOnStartup"=dword:00000000
"CopilotShowTips"=dword:00000000
"CopilotFeedback"=dword:00000000
"CopilotDataCollection"=dword:00000000

[HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced]
"EnableCopilot"=dword:00000000

[HKEY_CURRENT_USER\Software\Policies\Microsoft\Windows\WindowsCopilot]
"TurnOffWindowsCopilot"=dword:00000001

[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\WindowsCopilot]
"TurnOffWindowsCopilot"=dword:00000001

[HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced]
"TaskbarCopilot"=dword:00000000
