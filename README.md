
# Multipass on Windows 

# 1. What is Multipass? 

[Multipass](https://multipass.run/) is a CLI to launch and manage VMs on Windows, Mac and Linux that simulates a cloud environment with support for cloud-init. Get Ubuntu on-demand with clean integration to your IDE and version control on your native platform.

# 2. How to install multipass? 

You can install multipass from **[website](https://multipass.run/install)** or with **[Choco](https://chocolatey.org/install)**

# 3 . Installing **Choco**

Open powershell as administrator (or like a user) and run 

**# Get-ExecutionPolicy**

If you get a reply like ** Restricted** then run 

**#  Set-ExecutionPolicy AllSigned** 

Now paste command to your shell and press enter 

**# Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))**

For checking installation run 

**# choco**

If you get this page then go to forward 

![img](multipass2.png)

Ok , we installed **Choco** and now we can install **Multipass**

Run command below for installing multipass 

**# choco install multipass**

![img](multipass.png)

**BINGO**

Now we can run our ubuntu on multipass 

**# multipass shell**

![img](multipass3.png)
