# Low cost VPS: is $1.83/month real, will the renewal price double, and how much RAM do you actually need? (RackNerd plan table plus a per-GB RAM comparison)

$1.83 a month for a KVM VPS with 1 GB RAM, 20 GB SSD and 3 TB of transfer is the lowest price on the budget list I checked on November 13, 2026, and RackNerd lists that plan as renewing at the same rate rather than jumping in year two. Two catches come with the number: $1.83 is the monthly equivalent of a $21.96 one-year prepayment, and the server is unmanaged, so nothing gets installed or patched for you.

Below is what the three RackNerd tiers actually cost, how their renewal terms compare with the intro-price offers that dominate this price band, what 1 GB of RAM realistically runs, and the point at which a different provider is the better buy.

> **Quick pick**
> - Most readers, and anyone who just wants a cheap box to learn on, run a VPN or host a bot: **RackNerd 1 GB KVM at $1.83/mo equivalent, $21.96 paid once for the year.**
> - A small WordPress site or anything with concurrent visitors: **2 GB tier at $3.00/mo, $36.00 for the year, 2 vCPU and 35 GB SSD.**
> - Docker, several sites, or a 4 GB requirement: **the $5.00/mo tier with 3 vCPU, 60 GB SSD and 7 TB of transfer, $60.00 for the year.**
>
> 👉 [Check the current RackNerd 1 GB KVM price and order page](https://bit.ly/RacKnerd)

## RackNerd's three budget tiers side by side

| Plan | RAM / vCPU / Storage | Bandwidth | Price & term | Upfront / renewal | Order |
| --- | --- | --- | --- | --- | --- |
| 1 GB KVM VPS | 1 GB / 1 vCPU / 20 GB SSD | 3 TB | $1.83/mo on a 1-year term | $21.96 upfront, renews at the same price | [ Order the 1 GB KVM](https://bit.ly/RacKnerd) |
| 2 GB KVM VPS | 2 GB / 2 vCPU / 35 GB SSD | 5 TB | $3.00/mo on a 1-year term | $36.00 upfront, renews at the same price | [ Order the 2 GB KVM](https://bit.ly/RacKnerd) |
| $5.00 tier | 4 GB / 3 vCPU / 60 GB SSD | 7 TB | $5.00/mo on a 1-year term | $60.00 upfront, renews at the same price | [ Order the $5/mo 4 GB tier](https://bit.ly/RacKnerd) |

A word on the source of those figures. They come from a third-party price tracker that timestamps its tables (prices checked November 13, 2026), not from a RackNerd pricing page I could read directly. The 2 GB row matches what RackNerd's own specials page lists for that plan: 2 vCPU cores, 2 GB RAM, 35 GB SSD, 5 TB monthly transfer, 1 Gbps port, full root access, 1 IPv4 address, deployable in multiple locations. The 4 GB row sits in the same table and the page text credits RackNerd with the most RAM, cores and disk at the $5.00 mark, but treat the plan name as the list's label rather than an official SKU. Confirm the total and the renewal rate on the checkout page before you pay; small differences between a tracker and a live cart are normal.

RackNerd's specials page also settles a few things the price tables leave out. Every plan is KVM, unmanaged, includes full root access and one IPv4, and ships with **ctrl**, RackNerd's own control panel, which handles reboots, OS reinstalls, an HTML5 VNC console, one-click apps and an inbound firewall. Install images include CentOS, Rocky Linux, AlmaLinux, Fedora, Debian and Ubuntu, with custom ISO installs available through a support ticket. Support is listed as 24/7. That panel matters for the cost math below, because a bundled control panel is one line item you don't have to buy separately.

## Where cheap VPS pricing actually breaks: year two

Renewal is the number that decides whether a $2 plan stays a $2 plan. A2 Hosting's 2 GB self-managed plan advertises $3.49/mo, which requires $125.64 upfront on a three-year term, and then renews at $8.99/mo. Hostinger's KVM 1 shows $5.19/mo on a two-year term ($124.56 upfront) and renews at $11.99/mo. AccuWebHosting's VPS Edge goes from $4.84/mo to $9.77/mo. None of those are hidden; they're printed next to the intro price. They just don't appear in the headline.

| Provider | Plan | First-term price | Renewal price | Jump | Cash due at signup |
| --- | --- | --- | --- | --- | --- |
| RackNerd | 1 GB KVM | $1.83/mo (1 yr) | same price | 1.0× | $21.96 |
| RackNerd | 2 GB KVM | $3.00/mo (1 yr) | same price | 1.0× | $36.00 |
| A2 Hosting | Self Managed Linux 2GB | $3.49/mo (3 yr) | $8.99/mo | 2.6× | $125.64 |
| Hostinger | KVM 1 | $5.19/mo (2 yr) | $11.99/mo | 2.3× | $124.56 |
| AccuWebHosting | VPS Edge | $4.84/mo (2 yr) | $9.77/mo | 2.0× | $116.16 |
| IONOS | VPS S+ | $5.00/mo (1 yr) | $6.00/mo | 1.2× | $60.00 |
| Contabo | Cloud VPS 4 | $5.28/mo (2 yr) | $6.60/mo | 1.25× | $126.72 |

Two years on the RackNerd 1 GB plan costs $43.92 in total if the renewal rate holds, which is less cash than the single upfront payment A2, Hostinger, AccuWebHosting or Contabo ask for on day one. The trade is commitment length: RackNerd wants one year, those competitors want two or three to reach their advertised rate.

👉 [Lock in the 1 GB KVM at $1.83/mo with a one-year prepayment](https://bit.ly/RacKnerd)

One caveat on the "same price" claim: it's the tracker's标注 for these two plans, and it is the kind of term that gets changed. RackNerd's cancellation and refund terms weren't something I could verify from a primary page, so read them at checkout rather than assuming a money-back window exists. That's not a reason to skip the plan, but it is a reason to buy one year instead of three while you're testing whether the box suits you.

## The per-GB RAM view, and why it points the other way

Cheapest per month and cheapest per gigabyte of RAM are different contests. RackNerd's $1.83 lands at $1.83 per GB of RAM, which is fine at 1 GB and unremarkable at 4 GB. Once you need memory, the large instances win.

| Provider | Plan | RAM | Price | Per GB RAM |
| --- | --- | --- | --- | --- |
| Contabo | Cloud VPS 4 | 8 GB | $5.28/mo | $0.66 |
| AccuWebHosting | VPS Edge | 4 GB | $4.84/mo | $1.21 |
| Time4VPS | Linux 2 | 2 GB | $2.50/mo | $1.25 |
| Hostinger | KVM 1 | 4 GB | $5.19/mo | $1.30 |
| InterServer | 1 Slice | 2 GB | $3.00/mo | $1.50 |
| A2 Hosting | Self Managed Linux 2GB | 2 GB | $3.49/mo | $1.75 |
| RackNerd | 1 GB KVM | 1 GB | $1.83/mo | $1.83 |
| Namecheap | Spark | 1 GB | $3.88/mo | $3.88 |
| DigitalOcean | Basic 1 GB | 1 GB | $6.00/mo | $6.00 |

The rule I'd use: if 1 GB is genuinely enough for the workload, judge on the absolute monthly number, and RackNerd wins that by a wide margin against everything from $2.50 up. If you need 4 GB or 8 GB, judge on cost per GB and the budget-tier advantage mostly evaporates. Contabo's 8 GB instance at $5.28/mo is the value play in that column; it just isn't a 1 GB entry point, and its two-year term means $126.72 upfront.

## Is 1 GB enough? Match the tier to the job

Budget VPS specs cluster tightly: 1 to 4 GB RAM, one or two vCPUs, often on shared cores, and 20 to 50 GB of SSD or NVMe. Roughly 19 plans from 13 providers sit under $5/mo on the list I checked, which tells you how commoditized this tier is. What separates them is how much headroom you get for the same money.

- **1 GB, 1 vCPU**: a personal VPN endpoint, an IRC or Discord bot, a monitoring node, a sandbox for learning Linux, a single low-traffic static or near-static site. Plenty of RAM for the OS and one small service, nothing left over.
- **2 GB, 2 vCPU**: a small WordPress install with a cache in front of it, a lightweight database, a couple of containers. This is the tier where a control panel and a web server stop competing for memory. RackNerd's 2 GB tier is also the one the tracker labels as most vCPU for the money in its band.
- **4 GB, 3 vCPU**: WooCommerce, multiple sites on one box, Docker with a handful of services, a self-hosted app that expects headroom. RackNerd's $5.00 tier gives 3 vCPU and 60 GB of disk here, where several competitors at the same price cap out at 1 vCPU.

Bandwidth is rarely the binding limit at this level. Around 1 TB/month is the usual allowance for a public site, and these plans list 3 to 7 TB, so the constraint you'll hit first is RAM or CPU, not transfer. What you should check on any budget box is the fair-use clause and overage handling, since a "3 TB" figure with a strict fair-use rule behind it is not the same as 3 TB of guaranteed throughput.

Low-spec servers don't fail dramatically, they get slow. A 1 GB instance running WordPress plus a database plus a panel will spend its day swapping, and no amount of tuning fixes a memory ceiling. If the plan is a live site rather than a test, start at 2 GB.

## Costs that aren't in the headline price

The monthly rate is one line of a bill that can grow. Across budget hosting generally, these are the items that get added on:

- cPanel, Plesk or DirectAdmin licences (Liquid Web charges extra for cPanel, for example)
- automated backups and snapshots (IONOS sells backups separately; Namecheap's basic plan has no off-site backup storage)
- additional IPv4 addresses beyond the one included
- migration help moving an existing site or data over
- security add-ons such as malware scanning or DDoS filtering
- managed support on an unmanaged plan
- bandwidth overage or fair-use enforcement

RackNerd's structure avoids the first one: the bundled panel is ctrl, its own, not a licensed cPanel seat. There's no cPanel line on the specials page. If you specifically need cPanel, ask before ordering rather than assuming it's available. Backups are the item to plan around. Nothing on the pages I checked says automated backups are included with these specials, and on a self-managed box the working assumption should be that you keep your own off-site copies from day one. A $21.96 server with no backup discipline is a $21.96 server plus whatever your data was worth.

Refund windows in this market vary from generous to nonexistent, which is why the terms matter more than the price. Hostwinds runs a three-day return policy and doesn't include an SSL certificate; DigitalOcean states plainly that it doesn't refund. RackNerd's cancellation and refund terms weren't verifiable from a primary source during this check, so read the checkout page and the terms page before you pay, and size your first commitment to what you can afford to lose if the box doesn't fit.

👉 [See the RackNerd plan list and current checkout totals](https://bit.ly/RacKnerd)

## When a cheap RackNerd VPS is the wrong purchase

Skip unmanaged VPS hosting entirely, RackNerd included, if any of these describe you:

- **You don't want to touch a command line.** Unmanaged means you handle updates, the firewall, the web server and the database. A managed plan or shared hosting costs more and does that work for you.
- **The site is small and static.** A low-traffic brochure site doesn't need root access, and shared hosting will be cheaper once you price in your own time.
- **You need Windows.** RackNerd's specials page lists Linux images; nothing there confirms Windows availability on these plans.
- **You need physical isolation or a fully managed environment.** A dedicated server or a managed VPS is the correct product.
- **You need 8 GB of RAM on the smallest possible budget.** Contabo's Cloud VPS 4 at $5.28/mo for 8 GB and 4 vCPU, or AccuWebHosting's 4 GB VPS Edge at $4.84/mo, are better value per gigabyte. Both carry two-year terms and renew higher.

The other side of that list is where these plans earn their place: you want root, traffic is growing, you're running more than one site or app, or you need something between shared hosting and a dedicated box. Game servers, staging environments, private mail, teaching sandboxes and proxy endpoints all fit comfortably in this class of hardware.

## What to order, and what to check before you pay

Match the tier to the workload and stop there. Need a cheap Linux box to learn on, run a VPN or host a bot? The 1 GB KVM at $1.83/mo equivalent, $21.96 for the year, is the cheapest verified entry point and the renewal doesn't punish you. Running WordPress or expecting concurrent traffic? Go to 2 GB and 2 vCPU for $36.00 a year; the extra gigabyte is the difference between a site that loads and a site that swaps. Docker, multi-site, or anything that wants 4 GB? The $5.00/mo tier with 3 vCPU, 60 GB SSD and 7 TB is the one, at $60.00 for the year.

Before you enter card details, check two things on the order page: the total charged today including any add-ons you selected, and the renewal amount and refund terms for the plan. Then keep your own backups from the first hour.

👉 [Start with the RackNerd 1 GB KVM plan at $1.83/mo](https://bit.ly/RacKnerd)

## FAQ

**Is $1.83 a month a real monthly price?**
No. It's the monthly equivalent of $21.96 paid once for a one-year term. There's no verified monthly billing option for this plan in the data I checked, so budget the full year up front.

**Will the renewal price go up?**
The price tracker lists both the 1 GB and 2 GB plans as renewing at the same price, which is unusual in this band and the main reason they're worth a look. Confirm the renewal figure on the checkout page, since that's the version that governs your account.

**Can I run WordPress on 1 GB of RAM?**
It will boot and serve pages, but WordPress with a database and a control panel on 1 GB leaves almost nothing for traffic spikes. The 2 GB tier at $3.00/mo is the sensible floor for a live WordPress site.

**What's included besides the server?**
Full root access, one IPv4 address, a 1 Gbps port, the ctrl control panel with reboots, OS reinstall, an HTML5 VNC console, one-click apps and an inbound firewall, plus a choice of Linux distributions. It's unmanaged, so the software stack on top is yours to run.
