# splunk

### Windows

``` 
[WinEventLog://Security]
    renderXml = true
    disabled = false
    evt_resolve_ad_obj = true
    blacklist1 = EventCode="4662" Message="Object Type:\s+(?!groupPolicyContainer)"
    blacklist2 = EventCode="566" Message="Object Type:\s+(?!groupPolicyContainer)"
    blacklist3 = EventCode="4688" Message="New Process Name: (?i)(?:[C-F]:\Program Files\Splunk(?:UniversalForwarder)?\bin\(?:btool|splunkd|splunk|splunk-(?:MonitorNoHandle|admon|netmon|perfmon|powershell|regmon|winevtlog|winhostinfo|winprintmon|wmi)).exe)"
    index = windows 

[WinEventLog://Application]
    renderXml = true
    disabled = false
    index = windows 

[WinEventLog://System]
    renderXml = true
    disabled = false
    index = windows

[WinEventLog://Microsoft-Windows-Sysmon/Operational]
    renderXml = true
    disabled = false
    index = windows

[WinEventLog://Microsoft-Windows-WindowsUpdateClient/Operational]
    renderXml = true
    disabled = false
    index = windows

[WinEventLog://Microsoft-Windows-Windows Firewall With Advanced Security/Firewall]
    renderXml = true
    disabled = false
    index = windows

[WinEventLog://Microsoft-Windows-TerminalServices-LocalSessionManager/Operational]
    renderXml = true
    disabled = false
    index = windows

[WinEventLog://Microsoft-Windows-Windows PowerShell]
    renderXml = true
    disabled = false
    index = windows

[WinEventLog://Microsoft-Windows-Windows-PowerShell/Operational]
    renderXml = true
    disabled = false
    index = windows

[WinEventLog://Microsoft-Windows-WMI-Activity/Operational]
    renderXml = true
    disabled = false
    index = windows

[WinEventLog://Microsoft-Windows-TaskScheduler/Operational]
    renderXml = true
    disabled = false
    index = windows

[WinEventLog://Microsoft-Windows-Winlogon/Operational]
    renderXml = true
    disabled = false
    index = windows

[WinEventLog://Microsoft-Windows-SMBServer/Operational]
    renderXml = true
    disabled = false
    index = windows

[WinEventLog://Microsoft-Windows-WLAN-AutoConfig/Operational]
    renderXml = true
    disabled = false
    index = windows

[WinEventLog://Microsoft-Windows-Dhcp-Client/Operational]
    renderXml = true
    disabled = false
    index = windows  
```
