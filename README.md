# Windows VPS Asia: Hong Kong, Tokyo or Singapore, Which Windows Version You Need, and What $2.99–$47.99 a Month Buys (Full Plan Table + Price Benchmarks)

A 1 vCPU / 1 GB Windows VPS in Asia is listed at $4.50 a month by one provider and at $14.80 by another. One Hong Kong host puts both $14.80 and $20.80 on the same spec, on the same page, without explaining the gap. City, Windows edition and the way bandwidth is counted explain most of that spread. Core count explains very little of it.

Evoxt sits at the cheap end of the Asian market: Windows plans start at **$2.99/month** for 512 MB and **$5.99/month** for 1 vCore with 2 GB, running out of Hong Kong and Osaka on its premium network and Tokyo, Malaysia and Australia on the standard one. What follows is the full plan grid, the point where the low price stops being low, and a price cross-section against what the rest of the region lists.

> **Most readers should take VM-1 at $5.99/month.** 1 vCore, 2 GB RAM, 20 GB storage covers one ASP.NET site, a small SQL Server Express database, or an RDP desktop you actually log into. Step up to VM-2 ($11.99, 2 vCore / 4 GB) when SQL Server or a JVM is involved, and to VM-4 ($23.99, 4 vCore / 8 GB) for a production app with concurrent users.
>
> 👉 [See Evoxt's current Windows VPS plans and monthly pricing](https://bit.ly/EvoXt)

## The full Evoxt Windows VPS line-up

Eight plans, all priced in USD per month. Every VM includes a weekly offsite backup at no extra charge, a browser-based VNC console, firewall rules you can edit without logging into Windows, VM cloning and IP reassignment between servers.

| Plan | vCPU · RAM | Storage | Price (USD/mo) | Order |
| --- | --- | --- | --- | --- |
| VM-0.5 | 1 vCore · 512 MB | 5 GB | $2.99 | [ Order VM-0.5](https://bit.ly/EvoXt) |
| VM-0.75 | 1 vCore · 1 GB | 10 GB | $4.99 | [ Order VM-0.75](https://bit.ly/EvoXt) |
| VM-1 | 1 vCore · 2 GB | 20 GB | $5.99 | [ Order VM-1](https://bit.ly/EvoXt) |
| VM-1.5 | 2 vCore · 2 GB | 20 GB | $6.95 | [ Order VM-1.5](https://bit.ly/EvoXt) |
| VM-2 | 2 vCore · 4 GB | 30 GB | $11.99 | [ Order VM-2](https://bit.ly/EvoXt) |
| VM-4 | 4 vCore · 8 GB | 60 GB | $23.99 | [ Order VM-4](https://bit.ly/EvoXt) |
| VM-6 | 8 vCore · 8 GB | 60 GB | $29.99 | [ Order VM-6](https://bit.ly/EvoXt) |
| VM-8 | 8 vCore · 16 GB | 80 GB | $47.99 | [ Order VM-8](https://bit.ly/EvoXt) |

Resources can also be bought à la carte inside the VM control panel instead of by jumping a tier:

| Add-on | Price |
| --- | --- |
| Extra vCore | $3/month |
| Extra 1 GB RAM | $2/month |
| Extra IPv4 address | $3/month |
| Extra transfer, standard network | $3/TB |
| Extra transfer, premium network (Hong Kong, Osaka) | $12/TB |
| Extra transfer, Premium Plus | $24/TB |

Two pieces of arithmetic matter here. Moving from VM-4 to VM-6 costs $6 and gives you four more cores; buying those cores individually at $3 each would cost $12. Going the other way, if you are short on memory rather than cores, VM-4 plus 8 GB of add-on RAM lands at $39.99 for 4 vCore / 16 GB, against $47.99 for VM-8 with 8 vCore / 16 GB. Pick the VM-6 or VM-8 route when parallel throughput is the bottleneck, and stack RAM when it isn't.

One plan to skip for Windows: **VM-0.5**. 512 MB is under the practical floor for Windows Server with a desktop, so treat it as a Linux or utility box rather than a cheap RDP machine.

## Which of Evoxt's Asian locations to pick

Evoxt splits its regions into two groups. Standard covers Tokyo, Malaysia and Australia, alongside the US, UK, Canada, Germany, Poland and Amsterdam. Premium Network covers Hong Kong and Japan (Osaka). Plan prices are the same in both groups; the bandwidth economics are not.

Match the city to where your users actually are. Hong Kong is the closest of these locations to mainland China traffic, which makes it the default for cross-border SaaS and anything serving users in the Pearl River Delta. Tokyo or Osaka suits workloads whose users or upstream APIs sit in Japan. Malaysia fits Singapore-adjacent Southeast Asian audiences without the Singapore price tag that some hosts charge.

The pricing page doesn't publish latency tables, so pick by audience geography and measure once the VM is up. What it does publish is the overage rate, and that is where location turns into money: Hong Kong and Osaka bill extra transfer at **$12/TB**, four times the $3/TB standard rate. A service that pushes a couple of terabytes a month through Hong Kong is paying for the routing whether or not it needs it.

## The "unlimited bandwidth" promise that stops at Asia's edge

Read the asterisk before you read the price. Regxa advertises "Truly Unlimited Bandwidth" and then limits it in the footnote to the USA, Europe and the Middle East, with Asian locations (Singapore, India, Sydney) on plan-based allocation instead. OVHcloud's unlimited traffic carries the same carve-out: excluding datacentres in Asia-Pacific.

Evoxt takes the other approach and puts a number on the overage rather than a promise on the headline. That is easier to budget against, and it makes the region choice explicit: the same plan in Hong Kong costs four times as much per excess terabyte as it does in Tokyo. If your egress is small (a control panel, an internal tool, a few hundred GB), none of this matters. If you are streaming, proxying or serving large media, add up the monthly transfer first and treat the plan price as the smaller half of the bill.

## Windows Server version is a harder gate than CPU count

Cheap Asian Windows VPS plans often ship an old template library. One Hong Kong provider lists only Windows 2012 and 2016. Regxa offers 2022 and 2019 Datacenter with GUI or Core installs. Lightnode covers 2022, 2019 and 2016. If your application targets .NET 6, 7 or 8, or SQL Server 2022, a 2016-only template means hours of patching before your first deploy, and 2012 is out of support entirely.

Evoxt lists Windows RDP among its operating system options, but the plan and Windows pages don't enumerate which Server builds are in the template list, and they don't break out the licence as a separate line item on the plan price. Both are worth settling in writing with support before you pay, especially if you're comparing against a host that states "Windows Server included" directly on the plan card.

👉 [Check the Evoxt Windows VPS plan page before you order](https://bit.ly/EvoXt)

## What the rest of the Asian market lists

Same specs, different cities, wildly different numbers. None of these are links; the point is the spread, not the shopping list.

| Spec | Provider and location | Listed price |
| --- | --- | --- |
| 1 vCPU / 1 GB | asia.cloud, Hong Kong | $14.80 and $20.80, two columns on one page |
| 1 vCPU / 1 GB / 30 GB NVMe | regxa, Asia | $4.50/mo |
| 1 vCore / 1 GB / 10 GB | Evoxt, standard regions | $4.99/mo |
| 1 vCPU / 2 GB / 50 GB, dedicated CPU | lightnode, Seoul | $21.20/mo |
| 2 vCPU / 4 GB / 60 GB NVMe | asiawebhost, Singapore | S$55.00/mo |
| 2 vCPU / 4 GB / 120 GB NVMe | regxa, Asia | $15.00/mo |
| 2 vCore / 4 GB / 30 GB | Evoxt, standard regions | $11.99/mo |
| 4 vCores / 8 GB / 75 GB NVMe | OVHcloud VPS-2, Asia, ex. GST | US$8.50/mo |
| 4 vCore / 8 GB / 60 GB | Evoxt, VM-4 | $23.99/mo |

Four things distort that table. Currency and tax: asiawebhost bills in SGD, OVHcloud quotes excluding GST. Uptime definitions: asia.cloud sells a "100% network SLA" that covers the network only, regxa lists 99%, OVHcloud 99.9%, lightnode 99.95%, so the percentages are measuring different things. Licensing: OVHcloud's own footnote excludes Windows from Local Zones, so the US$8.50 entry price may not be a Windows price at the location you want. And virtualisation: lightnode's Seoul plans are dedicated-CPU, which is why a 1 vCPU / 2 GB box there costs more than a 2 vCPU / 4 GB box elsewhere.

## Billing, currency, and what to ask before you pay

Evoxt bills in USD, with terms from monthly out to three years, and lets you top up account credit for the system to draw down on future invoices. Payment runs through credit and debit cards, PayPal, Bitcoin and USDt on Tron.

Term length is the real cost lever. Hourly billing, as lightnode offers, suits a two-week migration test and costs almost nothing if you destroy the VM on Friday. Monthly with no contract, as asiawebhost runs, suits anything whose traffic you can't forecast. A multi-year prepay only makes sense for a workload you expect to keep, and the pages reviewed for Evoxt don't spell out a refund window or a pro-rated cancellation policy, so ask for the cancellation terms in writing before committing beyond a month. Regxa, for contrast, states a pro-rated refund on unused service time directly on its product page.

## FAQ

**Is the Windows licence included in the monthly price?**
Evoxt sells these as Windows VPS plans at a single monthly figure rather than a base price plus a Windows surcharge, which is how the plan cards read. Get written confirmation that the licence stays bundled for the life of the VM, because a per-month licence fee added later changes the comparison against hosts that state inclusion explicitly.

**Can I run SQL Server on the cheaper plans?**
2 GB (VM-1, $5.99) is enough for SQL Server Express with a small database and few connections. A standard edition instance with real users wants 8 GB, which means VM-4 at $23.99, or VM-2 plus 4 GB of add-on RAM at $19.99 if two cores will do. SQL Server's memory floor is the constraint, not the vCPU count.

**What happens if I exceed the transfer allowance?**
You are charged per terabyte: $3 on the standard network, $12 on premium (Hong Kong, Osaka), $24 on Premium Plus. Because Hong Kong is a premium location, a bandwidth-heavy deployment there pays four times the standard rate for every excess terabyte.

**Can I pay month to month?**
Yes. Billing terms run from monthly up to three years, so there's no obligation to prepay to get a Windows VM running.

**Which location for users in mainland China?**
Hong Kong. It's the nearest of Evoxt's Asian regions to the mainland and sits in the premium network group.

## Choosing between the plans

The decision collapses quickly. An RDP desktop and one small site: **VM-1 at $5.99**. SQL Server Express, IIS and a handful of users: **VM-2 at $11.99**, or VM-1 plus 2 GB of RAM at $9.99 if you want to stay on one core. A production .NET application with concurrent users: **VM-4 at $23.99**, adding RAM at $2/GB before jumping to VM-8. Anything that needs eight cores rather than eight gigabytes: VM-6 at $29.99 is $6 well spent over VM-4.

Two things to confirm at checkout: the Windows Server build in the template list, and the monthly transfer allowance for the region you chose, since Hong Kong and Osaka meter overage at four times the Tokyo rate.

👉 [Start with Evoxt's VM-1 at $5.99/month and confirm the Windows build before you deploy](https://bit.ly/EvoXt)
