# Week 2: How I solve problems

[← Home](../README.md)

## The Challenge
During my ESP lesson with Pete, We ran into a weird network issue where no one could ping their workstation at all, yet we were still able to Remote Desktop (RDC) straight into it without any problems.

## What We Did to Fix It
Since Remote Desktop was working fine, I knew the connection and IP address were fine, which meant something on the machine was specifically blocking ping requests.

1. So I logged into the workstation via Remote Desktop.
2. Then I went straight to the Firewall settings to check the inbound rules and see what was blocking the connection.
3. After looking through the setup, I found the specific application/rule that was stopping the machine from responding to pings and disabled it so traffic could get through.

## Looking Back at it Now
Checking the firewall worked straight away because I didn't waste time checking cables or resetting the network when I already knew RDC worked.

The best thing I got was pattern recognition. Since I know which firewall rule caused the block, I'll remember it immediately if it happens again. Being able to figure out a solution once and apply that pattern to future problems speeds up my troubleshooting alot.
