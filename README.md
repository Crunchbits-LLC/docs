# Crunchbits Documentation

> Welcome to Crunchbits' documentation and knowledgebase. 

## Getting Started
Click here to follow our basic getting started guide for a simple walk-through of our virtualized platform

## Frequently Asked Questions
List of more updated FAQ starts here

- Does Crunchbits have nested virtualization enabled by default?
    - Yes, every KVM and vDedicated(Smart Server / Instant Dedicated) we offer has nested virtualization enabled by default and uses host-passthrough KVM for maximum customer performance and compatibility.
- Does Crunchbits support custom rDNS entries on VPS plans?
    - Yes we do. You can modify rDNS records yourself and they will be instantly updated automatically, pending time for the records to become propagated. Look in our How-To's section or search for how to modify your rDNS record(s).
- My package came with 1Gbps bandwidth, why does my panel say 125MBps?
    - 125MB/s (or megabytes per second) is equivalent to 1Gbps (gigabits per second). MB/s (or MBps) are commonly confused with Mbps (megabits per second) which are not the same. Take a look at this handy conversion tool to learn a lot more.
- What are Crunchbits' policies around bandwidth and overages on my VPS?
    - If your VPS goes over its allocated bandwidth, the server will be automatically throttled to 625kB/s until your monthly allocated resources reset. We will not automatically suspend or terminate your account for bandwidth overages. If you are on a quarterly (or longer) billing cycle and contact us ahead of time, we can make one-time exceptions to bandwidth limitations to assist you in setting up, relocating, or backing up services to welcome you to Crunchbits.
- Does Crunchbits support IPv6?
    - Yes. All VPS's natively come with a /64. If you need an IPv6 allocation for your dedicated server, just contact technical support and let us know.
- Does Crunchbits support Windows ISOs on their VPS plans?
    - Yes, Crunchbits allows customers to install Windows on their VPS (as long as it is 2GB RAM or higher). Crunchbits **does not** provide licensing for any version of Windows and we do not provide any technical support related to Windows. You should be prepared to have a strong working knowledge of how to install, configure, and administer a remote Windows installation. We do provide multiple Windows ISOs for customers.
<details>
<summary>- What ISO's or Operating Systems are available to install on my VPS?</summary>
    - The following Operating systems are available:
        - AlmaLinux
        - 8 Minimal
        - 9 Latest

        - CentOS
        - 7 Minimal
        - Stream 9

        - Debian
        - Debian 10 (Buster) Minimal
        - Debian 11 (Bullseye) Minimal

        - Fedora
        - Fedora 34 Minimal
        - Fedora 35 Minimal
        - Fedora 36 Minimal

        - Rocky Linux
        - Rocky Linux 8 Minimal

        - Ubuntu
        - Ubuntu Server 18.04 LTS
        - Ubuntu Server 20.04 LTS
        - Ubuntu Server 22.04 LTS

        - Windows
        - Windows Server 2019 Standard
        - Windows Server 2019 Datacenter
        - Windows Server 2022 Standard
        - Windows Server 2022 Datacenter
</details>
<details>
<summary>- Yearly Fair Use CPU Usage</summary>
The yearly plans are not dedicated, but yes you can actually use the cores allotted. These plans are promotional and non-standard to our regular offerings, so this does not apply to our standard VPS and VDS product line-up.

Fair share CPU Usage (if the usage looks like abuse, we will suspend and contact you).

The standard operating procedure for this:
1. If you're a power user, and on a node with a lot of other power users, we'll quietly migrate you around to balance it out if the hypervisor looks a bit too busy for our ability to sleep comfortably at night.
2. If you're using a lot more than your peers, continually, we'll contact you and give you a heads up if it's a problem.
3. If you're non-responsive to that, we'll suspend you until we get a reply.

A safe number: no more than 25% continual load on your cores. At or under that, you'll never hear from us.
Questionable: Somewhere in between 25% and 75% load
An unsafe number: 75%+ load

We won't sugarcoat it: these plans are not meant to compete with our existing premium product stack. It's older hardware, slower drives, less capacity, and will be busier nodes. All things that do not apply to our standard product lineup. Will that matter for anyone who isn't crypto-mining or running a million-dollar e-commerce website? No. But if you're closer to that end of the spectrum definitely look at our VPS and VDS products.
</details>