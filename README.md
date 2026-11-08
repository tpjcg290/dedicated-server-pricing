# Dedicated server hosting price: what does bare metal cost per month, which plan do you actually need, and what gets added to the bill? (SpinServers' four plans and a four-provider price check)

A single-tenant server runs from **$79 a month** at the entry level to roughly **$680 a month** for a high-memory, multi-drive machine. That's the full spread of SpinServers' four published plans. Elsewhere the market stretches wider: around €25 a month for a small European box, $145 for a 24-core machine at PureVoltage, $218.98 for a managed InMotion config with cPanel bundled, and past €600 for current-generation AMD hardware with a lot of RAM.

Three line items push that number up after you pick a plan: control panel licensing, backup storage, and the bandwidth cap. Below is what each SpinServers plan includes, what it leaves you to buy separately, and where the same money buys more elsewhere.

> **Quick answer.** The **$79 Xeon E3-1280 v5 plan** (4 cores, 32GB RAM, 1TB NVMe, 30TB transfer on a 10Gbps port) covers a single busy site or a small stack of them. Move to the **$149 Growth plan** when you need 256GB of RAM or RAID-1 storage. Both are month-to-month, and the three packaged plans carry no setup fee.
> 👉 [Check current SpinServers dedicated server pricing](https://bit.ly/Spinservers)

## SpinServers plans and prices

Four plans carry a published monthly rate. All are bare metal with root access, deployed in Dallas or San Jose, and provisioned automatically within minutes of payment.

| Plan | CPU | RAM / storage | Bandwidth and port | Price | Order |
| --- | --- | --- | --- | --- | --- |
| Intel Xeon E3-1280 v5 | 4 cores / 8 threads | 32GB DDR4 ECC / 1TB NVMe | 30TB on 10Gbps (2×10Gbps ports listed) | **$79/mo**, monthly | [Check the $79 plan](https://bit.ly/Spinservers) |
| Starter Package | 4-core Xeon E3-1280 v5 | 32GB DDR4 / 1TB M.2 NVMe | 10TB on 10Gbps | **$99/mo**, month-to-month, no setup fee | [Check the Starter plan](https://bit.ly/Spinservers) |
| Growth Package | 2× Xeon E5-2630L v3 (16 cores / 32 threads) | 256GB DDR4 / 2×1.6TB SSD, RAID-1 | 20TB on 10Gbps | **$149/mo**, month-to-month, no setup fee | [Check the Growth plan](https://bit.ly/Spinservers) |
| High Performance Package | 4× Xeon E5-4640 v2 | 768GB RAM / 8×2TB SSD, RAID-10 | 40TB on 10Gbps | **$679/mo**, month-to-month, no setup fee | [Check the High Performance plan](https://bit.ly/Spinservers) |

Two things in that table are worth pausing on.

The **$79 and $99 plans list the same processor and the same 32GB of RAM**, so the extra $20 isn't buying compute. It buys a different bandwidth allowance and contract terms, and in this case the cheaper plan actually lists the larger allowance (30TB against 10TB). If transfer volume matters more to you than a support arrangement, the entry plan is the better buy on paper. Confirm the final figures at checkout, because allocations shift with location and hardware availability.

The **$679 plan is a memory-and-drives purchase, not a compute purchase**. Four E5-4640 v2 chips and DDR3 memory are old platform technology. PureVoltage sells a 24-core EPYC 7443P with 256GB DDR4 and 100TB of transfer for $276 a month. You would choose the $679 tier for 768GB of RAM and eight SSD drives in RAID-10, and for nothing else.

The Dallas and San Jose product pages also list larger builds (a dual Xeon Platinum 8173M with 56 cores, 512GB RAM and 4×1.92TB SSD among them) without a published rate, so treat the four plans above as the priced menu and those bigger machines as quote-based.

### What comes with the plan, and what doesn't

| Included | Confirm before ordering |
| --- | --- |
| IPv4 address (IPv6 /64 on some configurations) | Control panel licence (cPanel or similar) |
| IPMI / iKVM remote management and OS reinstall | Managed support tier |
| Linux, Windows and ESXi auto-install | Backup storage |
| Instant provisioning in Dallas or San Jose | Bandwidth overage rate |
| DDoS-protected network, private Layer 2 VPC networking | Refunds on month-to-month service |

The hardware is Dell, HP and Supermicro class, and the facilities are advertised as PCI-compliant. SpinServers supplies the infrastructure, not the compliance work: managed PCI scanning and compliance support are not part of the offer, which matters if you're taking card payments and assumed the host would handle it.

## What actually drives the dedicated server hosting price up or down

Seven variables explain almost every quote difference you'll see between providers.

**CPU generation.** An E3-1280 v5 is a 2015-era Skylake chip. It's cheap per core and perfectly capable for a web server, but a current EPYC or Ryzen core does more work per clock. Old silicon is why entry prices sit under $100.

**Memory.** Going from 32GB to 256GB is the single biggest jump in the SpinServers lineup, and it accounts for most of the $70 gap between the entry plan and the Growth plan.

**Storage type and drive count.** NVMe costs more than SATA SSD, and RAID-10 with eight drives costs more than RAID-1 with two.

**Port speed against transfer cap.** A 10Gbps port is standard at this tier and mostly a burst number. The cap in terabytes is what you'll actually hit. Ten terabytes on the $99 Starter is thin for anything serving video or large downloads.

**Location.** Dallas and San Jose don't carry identical stock or identical rates, and SpinServers states that pricing varies by location, hardware and availability. Pick the facility nearest your users before you compare prices, since latency follows geography regardless of what you pay.

**Managed or unmanaged.** These four plans ship with root access and no management layer. A managed plan includes monitoring, security patching and human support, though not every provider that calls a plan managed actually staffs support around the clock.

**Add-ons.** DDoS protection beyond the baseline, backup space, software licences and extra IPs all land on the invoice separately at most hosts.

## The real monthly bill after the headline rate

Year one on the $79 plan costs **$948** if you stay month-to-month. The Growth plan runs **$1,788** a year, and the High Performance plan **$8,148**. No setup fee applies to the three packaged plans, so those figures are the full server cost.

The extras are where budgets drift.

**Control panel.** InMotion values the cPanel licence on its dedicated plans at $58.99 a month. That's a reasonable scale reference for what a panel adds over a year, and it's the line most people forget when comparing a bare-metal price against a managed one.

**Backup.** InMotion prices 500GB of backup storage at $90 a month and 2TB at $360 a month, again as stated value rather than a separate charge. SpinServers doesn't publish a backup rate alongside these plans. Ask for it in writing before you assume snapshots are included, because a RAID array protects against a dead disk and nothing else.

**Bandwidth overage.** Rates for exceeding the monthly cap aren't published on the plan listing. If you expect to run near 10TB or 20TB, get the per-terabyte overage figure first.

**Contract length.** PureVoltage discounts one- to three-year contracts and HOSTKEY cuts 10–25% off for six- to twelve-month commitments. SpinServers sells these plans month-to-month, which caps your exposure: you can leave after 30 days, and there's no scheduled renewal hike to plan around.

That last point is the difference between two kinds of price risk. InMotion's 24-core tier renews at **$238.98 a month** after the introductory term, a jump you can calculate in advance. SpinServers carries the opposite risk, where the rate you see depends on which location and hardware is available when you order. Month-to-month cuts both ways, and it generally means **no refund policy** on the service, so the first month is your evaluation period.

## Who shouldn't rent a dedicated server

InMotion says plainly that dedicated servers aren't the right fit for everyone and points smaller operations at VPS hosting. That's honest, and it applies here.

A site pulling a few thousand visits a day, a staging environment, a side project with a database: a $20–$50 VPS handles it, and you keep the $79. The break-even point sits where a VPS stops being reliable under load. HOSTKEY puts the dedicated-server threshold at large shops and news sites above roughly 20,000 daily visits, plus game servers, live streaming, large file storage and video platforms.

You also don't want bare metal if you have no one to administer it. These plans assume you can manage a Linux or Windows install, patch it, and debug it at 2am. If that's not you, a managed plan at a higher monthly rate is cheaper than an outage.

Finally, if managed PCI compliance is a hard requirement, look at a provider that sells compliance as a service rather than a colocation-style bare-metal host.

## Price check against three other providers

| Provider | Cheapest verified monthly rate | What it buys | Bandwidth | Contract notes |
| --- | --- | --- | --- | --- |
| SpinServers | **$79** | Xeon E3-1280 v5, 4c/8t, 32GB DDR4, 1TB NVMe | 30TB on 10Gbps | Monthly; no setup fee on packaged plans; no refund on month-to-month |
| PureVoltage | **$145** | Xeon E5-2680 v4, 24c/48t, 128GB DDR4, 1TB NVMe | 100TB on 10Gbps | No setup fees; discounts on 1–3 year terms |
| InMotion Hosting | **$218.98** | Xeon E-2388G, 8c/16t, 128GB DDR4, 2×1.92TB NVMe RAID-1, 16 IPs | 1Gbps unmetered | 12-month term; cPanel and 500GB backup bundled |
| HOSTKEY | ~**€25** entry, ~€100 typical | Varies by build; unmanaged by default | 1–10Gbps; inbound free, outbound per plan | 6–12 month contracts cost 10–25% less |

The pattern is clear enough. **SpinServers wins on entry price and on port speed at the bottom of the range**: nothing else here gives you a 10Gbps port and 30TB of transfer for under $80. **PureVoltage wins on cores per dollar** by a wide margin at $145, and its pricing is flat and transparent.

**InMotion's $218.98 is a different product**: a 12-month managed term with cPanel, backup and 16 IPs folded into the rate. Compare it against a SpinServers plan plus a cPanel licence plus backup and the gap narrows, though InMotion's 1Gbps unmetered port can't match 10Gbps for burst throughput.

**HOSTKEY is the Europe option.** Its published prices swing from roughly €25 to €600 depending on the build, and its bandwidth model charges outbound traffic by plan while inbound stays free. Worth checking if your users are in Germany or the Netherlands, where a few milliseconds of latency matter more than a few dollars.

## FAQ

**How much does a dedicated server cost per month?**
At SpinServers, $79 to $679 depending on configuration. Across the wider market, roughly €25 at the absolute entry level, $145 for a modern 24-core machine, and past $600 for high-core-count EPYC builds with large memory.

**Do I need cPanel on a dedicated server?**
Only if you or your clients expect a graphical interface for managing sites, email and DNS. cPanel licensing on a dedicated box is a real recurring cost, valued at $58.99 a month on InMotion's plans. Command-line administration and a free panel cover most single-application servers.

**Is a 10Gbps port worth paying for?**
It's included on every SpinServers plan here, so the question is whether the transfer cap fits. A 10Gbps port with a 10TB monthly cap is like a wide door with a small room behind it. Match the terabytes to your actual monthly egress before you get excited about the port speed.

**Will the price go up after the first term?**
SpinServers sells these plans month-to-month, so there's no introductory rate to expire. The variable is availability: prices vary by location, hardware and stock. Get the rate for your chosen facility confirmed in writing. Where a provider does publish a renewal figure, budget for it (InMotion's higher tier renews at $238.98 a month).

**Can I pay monthly, and can I get a refund?**
Yes to monthly on all four plans. The packaged plans carry no setup fee. Month-to-month service generally comes with no refund policy, so use the first billing cycle to test performance from your real traffic locations.

**Is a long contract worth the discount?**
If you're confident about staying put, yes. PureVoltage discounts one- to three-year terms and HOSTKEY cuts 10–25% for six to twelve months. SpinServers doesn't publish a term discount on these plans, so you're trading a lower rate for flexibility.

## How to choose

Match the plan to the workload rather than to the spec sheet.

**One high-traffic site, a CMS or an application server** → the $79 Xeon E3 plan. Thirty terabytes of transfer and a 10Gbps port at that price is the strongest entry offer in this comparison, and the CPU is more than adequate for a single site.

**Several sites, a database with a large working set, or anything that needs RAM headroom** → the $149 Growth plan. The 256GB of RAM and RAID-1 storage are what you're paying for; the CPU and bandwidth are not upgrades over the entry plan.

**Video delivery or large file hosting** → check the overage rate on the 30TB cap first, and compare against an unmetered option if your egress is genuinely heavy.

**cPanel, managed support and backups under one invoice** → InMotion at $218.98 on a 12-month term.

**Users in mainland Europe** → HOSTKEY, and run a latency test from Frankfurt or Amsterdam before you decide.

**Genuinely need 768GB of RAM and eight drives** → the $679 tier. Otherwise skip it; $276 buys a modern 24-core EPYC elsewhere.

Two things to confirm before you enter card details. First, that the quote matches the facility you actually want, since Dallas and San Jose stock different hardware at different rates. Second, the backup and control-panel line items and the per-terabyte overage rate, because those three are what turn an $79 headline into a $150 invoice.

👉 [Compare SpinServers' four dedicated server plans and current rates](https://bit.ly/Spinservers)
