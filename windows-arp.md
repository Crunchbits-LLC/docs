# Windows ARP Issues and Broken Connectivity

This is a vague connectivity issue that specifically applies to Windows OSes in a virtualized environment. Some of the symptoms may include (but are not limited to):

- You may see both a false duplicate and a preferred IP in the output
- Assigning an IP address, you see a duplicate IP address conflict
- Your Windows OS sporadically loses it's link to WAN and/or traceroutes die at the gateway (both from within your Windows VM and from outside coming in)

**Resolution**: Turn off gratuitous ARP in the Windows OS

To turn off gratuitous ARP in Windows:

1. Power on the virtual machine and log in.
2. Click Start, type <code>regedit</code>, and click <code>OK</code>.
3. Locate this registry key: <code>HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\Tcpip\Parameter</code>
4. Click **Edit > New**, and click DWORD Value.
5. Type <code>ArpRetryCount</code>.
6. Right-click the <code>ArpRetryCount</code> registry entry and click **Modify**.
7. In the Value box, type <code>0</code> and click <code>OK</code>.
8. Exit the Registry Editor.
9. Shut down the guest operating system and power off the virtual machine.
10. Power on the virtual machine.
11. Connectivity should be restored.
This is an issue specific to any only involving Windows. While we offer unmanaged services, we will attempt to help you troubleshoot with best-effort when we're available on our part.