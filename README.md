# EBDP
EternalBlue / DoublePulsar

Having some fun.

## Personalize your OWN

The binary itself will check if an XML file exists with the same filename of the executable
(clearly without extension)

**For example**: *EternalBlue.exe* will look in the same directory for: *EternalBlue.xml*

(same for *DoublePulsar* obv)


## XML Required Values
  
#### EternalBlue exploit
  *(Input parameters, before exploitation)*
  - NetworkTimeout : replace *%TIMEOUT%* with your fav timeout sec. value
  - TargetIp : replace *%TARGET_IP_ADDRESS* with your target IP address
  - TargetPort : replace *%TARGET_SMB_PORT%* with your target's opened SMB port
  - Target : replace *%TARGET_OPERATING_SYSTEM* with your target's operating system (see notice)
  
  Other interesting parameters:
  - VerifyTarget
  - VerifyBackdoor
  - MaxExploitAttempts
  - DaveProxyPort
  
  Other:
  - GroomAllocations
  - ShellcodeBuffer
  
 
  *(Output parameters, after exploitation)*
  - DoublePulsarPresent
  
  **NOTICE FOR TARGET**:
  Target's possible values:
  * **XP** for *Windows XP*
  * **WIN72K8R2** for *Windows 7* / *Windows Server 2008* / *Windows Vista*
   
#### DoublePulsar backdoor
  *(Input parameters, before payload execution)*
  - NetworkTimeout : replace *%TIMEOUT%* with your fav timeout sec. value
  - TargetIp : replace *%TARGET_IP_ADDRESS* with your target IP address
  - TargetPort : replace *%TARGET_PORT%* with your target's opened port
  - Protocol : replace *%PROTOCOL%* with your protocol of choice (see notice)
  - Architecture : replace *%TARGETARCHITECTURE%* with target arch. (see notice)
  - Function : replace *%FUNCTION_VALUE%* with desired operation (see notice)
  
  *(Output parameters, after payload execution)*
  - OutputInstall
  - Ping
  - RunDLL
  - Uninstall
  
  **#1 NOTICE FOR PROTOCOL**:
  Protocol's possible values:
  * **SMB** for *Server Message Block* protocol
  * **RDP** for *Remote Desktop Protocol* protocol
  
  **#2 NOTICE FOR ARCHITECTURE**:
  Architecture's possible values:
  * **x86** for *x86*-based processors
  * **x64** for *x86* with 64-bit extension processors
  
  **#3 NOTICE FOR FUNCTION**:
  Function's possible values:
  * **OutputInstall** to output install shellcode file
  * **Ping** to check if backdoor is installed
  * **RunDLL** to inject DLL to a process
  