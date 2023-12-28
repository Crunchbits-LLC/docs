# Crunchbits Knowledge Base & Documentation

> Welcome to Crunchbits' documentation and knowledge base.

## Getting Started
Click [here](Using-the-basic-functions-of-the-server) to follow our basic getting started guide for a simple walk-through of our virtualized platform.

---

# Frequently Asked Questions

<details><summary style="color: var(--theme-color,#ea6f5a); font-weight: 600;">Does Crunchbits have nested virtualization enabled by default?  </summary>
<p style="    display: block;
    margin-block-start: 1em;
    margin-block-end: 1em;
    margin-inline-start: 40px;
    margin-inline-end: 40px;
    border-left: 4px solid var(--theme-color,#ea6f5a);
    margin: 2em 0;
    padding-left: 20px;">Yes, every KVM and vDedicated (Smart Server / Instant Dedicated) we offer has nested virtualization enabled by default and uses host-passthrough KVM for maximum customer performance and compatibility.</p>
</details>
&nbsp;
<details><summary>**Does Crunchbits support custom rDNS entries on VPS plans?**  </summary>
Yes we do. You can modify rDNS records yourself and they will be instantly updated automatically, pending time for the records to become propagated. Look in our How-To's section or search for how to modify your rDNA record(s).</details>
&nbsp;
<details><summary>My package came with 1Gbps bandwidth, why does my panel say 125MBps?**  </summary>
125MB/s (or megabytes per second) is equivalent to 1Gbps (gigabits per second). MB/s (or MBps) are commonly confused with Mbps (megabits per second) which are not the same. Take a look at this handy conversion tool to learn a lot more.</details>
&nbsp;
<details><summary>What are Crunchbits' policies around bandwidth and overages on my VPS?**  </summary>
If your VPS goes over its allocated bandwidth, the server will be automatically throttled to 625kB/s until your monthly allocated resources reset. We will not automatically suspend or terminate your account for bandwidth overages. If you are on a quarterly (or longer) billing cycle and contact us ahead of time, we can make one-time exceptions to bandwidth limitations to assist you in setting up, relocating, or backing up services to welcome you to Crunchbits.</details>
&nbsp;
<details><summary>Does Crunchbits support IPv6?**  </summary>
Yes. All VPS's natively come with a /64. If you need an IPv6 allocation for your dedicated server, just contact technical support and let us know.</details>
&nbsp;
<details><summary>Does Crunchbits support Windows ISOs on their VPS plans?**  </summary>
Yes, Crunchbits allows customers to install Windows on their VPS (as long as it is 2GB RAM or higher). Crunchbits does not provide licensing for any version of Windows and we do not provide any technical support related to Windows. You should be prepared to have a strong working knowledge of how to install, configure, and administer a remote Windows installation. We do provide multiple Windows Server templates for customers.</details>

<style>
    
details {
  width: 75%;
  min-height: 5px;
  max-width: 700px;
  padding: 45px 70px 45px 45px;
  margin: 0 auto;
  position: relative;
  font-size: 22px;
  border: 1px solid rgba(0,0,0,.1);
  border-radius: 15px;
  box-sizing: border-box;
  transition: all .3s;
}

details + details {
  margin-top: 20px;
}

details[open] {
  min-height: 50px;
  background-color: #333333;
  box-shadow: 2px 2px 20px rgba(0,0,0,.2);
}

details p {
  color: #96999d;
  font-weight: 300;
}

summary {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-weight: 500;
  cursor: pointer;
}

summary:focus {
  outline: none;
  
}

summary:focus::after {
  content: "";
  height: 100%;
  width: 100%;
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  box-shadow: 0 0 0 5px rebeccapurple;
}

summary::-webkit-details-marker {
  display: none
}

.control-icon {
  fill: rebeccapurple;
  transition: .3s ease;
  pointer-events: none;
}

.control-icon-close {
  display: none;
}

details[open] .control-icon-close {
  display: initial;
  transition: .3s ease;
}

details[open] .control-icon-expand {
  display: none;
}
</style>

<details>
  <summary>
    Does Crunchbits have nested virtualization enabled by default?
    <svg class="control-icon control-icon-expand" width="24" height="24" role="presentation"><use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#expand-more" /></svg>
    <svg class="control-icon control-icon-close" width="24" height="24" role="presentation"><use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#close" /></svg>
  </summary>
  <p>Yes, every KVM and vDedicated (Smart Server / Instant Dedicated) we offer has nested virtualization enabled by default and uses host-passthrough KVM for maximum customer performance and compatibility.</p>
</details>

<details>

  <summary>
    Does Crunchbits support custom rDNS entries on VPS plans?
    <svg class="control-icon control-icon-expand" width="24" height="24" role="presentation"><use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#expand-more" /></svg>
    <svg class="control-icon control-icon-close" width="24" height="24" role="presentation"><use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#close" /></svg>
  </summary>
  <p>Yes we do. You can modify rDNS records yourself and they will be instantly updated automatically, pending time for the records to become propagated. Look in our How-To's section or search for how to modify your rDNA record(s).</p>
</details>

<details>
  <summary>
    My package came with 1Gbps bandwidth, why does my panel say 125MBps?    
    <svg class="control-icon control-icon-expand" width="24" height="24" role="presentation"><use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#expand-more" /></svg>
    <svg class="control-icon control-icon-close" width="24" height="24" role="presentation"><use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#close" /></svg>
  </summary>
  <p>125MB/s (or megabytes per second) is equivalent to 1Gbps (gigabits per second). MB/s (or MBps) are commonly confused with Mbps (megabits per second) which are not the same. Take a look at this handy conversion tool to learn a lot more.</p>
</details>

<details>
  <summary>
    What are Crunchbits' policies around bandwidth and overages on my VPS?
    <svg class="control-icon control-icon-expand" width="24" height="24" role="presentation"><use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#expand-more" /></svg>
    <svg class="control-icon control-icon-close" width="24" height="24" role="presentation"><use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#close" /></svg>
  </summary>
  <p>If your VPS goes over its allocated bandwidth, the server will be automatically throttled to 625kB/s until your monthly allocated resources reset. We will not automatically suspend or terminate your account for bandwidth overages. If you are on a quarterly (or longer) billing cycle and contact us ahead of time, we can make one-time exceptions to bandwidth limitations to assist you in setting up, relocating, or backing up services to welcome you to Crunchbits.</p>
</details>

<details>

  <summary>
    Does Crunchbits support IPv6?
    <svg class="control-icon control-icon-expand" width="24" height="24" role="presentation"><use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#expand-more" /></svg>
    <svg class="control-icon control-icon-close" width="24" height="24" role="presentation"><use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#close" /></svg>
  </summary>
  <p>Yes. All VPS's natively come with a /64. If you need an IPv6 allocation for your dedicated server, just contact technical support and let us know.</p>
</details>

<details>
  <summary>
    Does Crunchbits support Windows ISOs on their VPS plans?   
    <svg class="control-icon control-icon-expand" width="24" height="24" role="presentation"><use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#expand-more" /></svg>
    <svg class="control-icon control-icon-close" width="24" height="24" role="presentation"><use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#close" /></svg>
  </summary>
  <p>Yes, Crunchbits allows customers to install Windows on their VPS (as long as it is 2GB RAM or higher). Crunchbits does not provide licensing for any version of Windows and we do not provide any technical support related to Windows. You should be prepared to have a strong working knowledge of how to install, configure, and administer a remote Windows installation. We do provide multiple Windows Server templates for customers.</p>
</details>