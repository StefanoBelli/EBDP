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
  - NetworkTimeout : replace *%TIMEOUT%* with your fav timeout sec. value
  - TargetIp : replace *%TARGET_IP_ADDRESS* with your target IP address
  - TargetPort : replace *%TARGET_SMB_PORT%* with your target's opened SMB port
  - Target : replace *%TARGET_OPERATING_SYSTEM* with your target's operating system:
  
 Other interesting parameters:
  - VerifyTarget
  - VerifyBackdoor
  - MaxExploitAttempts
  - DaveProxyPort
  
 Other:
  - GroomAllocations
  - ShellcodeBuffer
  - DoublePulsarPresent
  
 **NOTICE FOR TARGET**:
  Target's possible values:
   * **XP** for *Windows XP*
   * **WIN72K8R2** for *Windows 7* / *Windows Server 2008* / *Windows Vista*