# Affordable VPS hosting: what $2.50 a month really buys, which plan fits WordPress or WooCommerce, and where the cheap price stops being cheap

Vultr's entry price is **$2.50/month** for 1 vCPU, 0.5 GB of RAM and 10 GB of SSD storage, but that specific plan is IPv6-only and deploys in two locations. The plan most readers should buy is the **$5/month** tier: 1 vCPU, 1 GB RAM, 25 GB SSD, 1 TB of bandwidth, a public IPv4 address and 31 data center regions to choose from. A single WordPress site runs comfortably at **$10/month**, and WooCommerce or a handful of sites starts at **$20**.

Below is the full current Vultr lineup with prices and hourly rates, followed by the part most "cheapest VPS" lists skip: what the headline price leaves out, how much server your workload actually needs, and the add-on charges that turn a $2 plan into a $15 bill.

> **Quick pick:** the **$5/month** Cloud Compute plan (1 vCPU, 1 GB RAM, 25 GB SSD, 1 TB bandwidth) is the smallest tier that gives you a normal IPv4 address and a real choice of regions. It handles a small WordPress site, a staging server, a VPN or a Discord bot. Skip the $2.50 tier unless you specifically want an IPv6 lab box.
> 👉 [Check the $5 Cloud Compute plan and its current price](https://www.vultr.com/pricing/?ref=9738262-9J)

## Vultr's full plan list, and who each tier is for

Vultr splits its compute into two lines that matter for budget buyers. Regular Performance runs previous-generation Intel CPUs on standard SSD and starts at $2.50. High Performance runs current AMD EPYC or Intel Xeon chips on NVMe and starts at $6.

The gap between those two entry points is smaller than it looks. The $6 High Performance plan gives you 1 GB of RAM, **2 TB of bandwidth** (double the $5 regular plan) and faster NVMe storage for one extra dollar. If you're already spending $5, the $6 plan is the better buy.

**Regular Performance** (previous-gen Intel, standard SSD):

| Plan (vCPU · RAM) | Storage | Bandwidth | Price | Deploy |
| --- | --- | --- | --- | --- |
| 1 · 0.5 GB, IPv6 only | 10 GB SSD | 0.50 TB | **$2.50/mo** ($0.004/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 1 · 0.5 GB | 10 GB SSD | 0.50 TB | **$3.50/mo** ($0.005/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 1 · 1 GB | 25 GB SSD | 1.00 TB | **$5/mo** ($0.007/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 1 · 2 GB | 55 GB SSD | 2.00 TB | **$10/mo** ($0.015/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 · 2 GB | 65 GB SSD | 3.00 TB | **$15/mo** ($0.022/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 · 4 GB | 80 GB SSD | 3.00 TB | **$20/mo** ($0.030/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 4 · 8 GB | 160 GB SSD | 4.00 TB | **$40/mo** ($0.060/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 6 · 16 GB | 320 GB SSD | 5.00 TB | **$80/mo** ($0.119/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 8 · 32 GB | 640 GB SSD | 6.00 TB | **$160/mo** ($0.238/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 16 · 64 GB | 1280 GB SSD | 10.00 TB | **$320/mo** ($0.476/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 24 · 96 GB | 1600 GB SSD | 15.00 TB | **$640/mo** ($0.952/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |

**High Performance** (AMD EPYC or Intel Xeon, NVMe SSD):

| Plan (vCPU · RAM) | Storage | Bandwidth | Price | Deploy |
| --- | --- | --- | --- | --- |
| 1 · 1 GB | 25 GB NVMe | 2.00 TB | **$6/mo** ($0.009/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 1 · 2 GB | 50 GB NVMe | 3.00 TB | **$12/mo** ($0.018/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 · 2 GB | 60 GB NVMe | 4.00 TB | **$18/mo** ($0.027/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 · 4 GB | 100 GB NVMe | 5.00 TB | **$24/mo** ($0.036/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 4 · 8 GB | 180 GB NVMe | 6.00 TB | **$48/mo** ($0.071/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 4 · 12 GB | 260 GB NVMe | 7.00 TB | **$72/mo** ($0.107/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 8 · 16 GB | 350 GB NVMe | 8.00 TB | **$96/mo** ($0.143/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 12 · 24 GB | 500 GB NVMe | 12.00 TB | **$144/mo** ($0.214/hr) | [Deploy](https://www.vultr.com/pricing/?ref=9738262-9J) |

Vultr's pricing page also lists High Frequency plans on newer Intel CPUs with NVMe; the two tables above cover the lines most buyers end up comparing.

Who each tier actually suits:

- **$2.50 and $3.50 (0.5 GB)**: throwaway test boxes, a proxy, a monitoring node. Not a website. Half a gigabyte of RAM runs MySQL and PHP badly, and the $2.50 plan has no IPv4 at all.
- **$5 Regular or $6 High Performance (1 GB)**: a static site, a small blog, a dev environment, a VPN. If you're on this tier, take the $6 High Performance plan — the extra dollar buys NVMe and doubles your bandwidth.
- **$10 / $12 (2 GB)**: one WordPress site with a normal plugin load. This is the realistic floor for WordPress.
- **$15 (2 vCPU, 2 GB)**: WordPress with real traffic, or a small app that needs a second core more than it needs RAM.
- **$20 (2 vCPU, 4 GB)**: WooCommerce, membership sites, or three or four small sites sharing one box.
- **$40 and up**: multi-site stacks, CI runners, game servers, databases that hold real data. Most readers of a "cheap VPS" article never need these.

👉 [Compare every Vultr Cloud Compute tier side by side](https://www.vultr.com/pricing/?ref=9738262-9J)

## The $2.50 sticker price has three catches

**No IPv4 address.** The $2.50 plan is IPv6-only, and Vultr says so on the pricing table. If any visitor, API client or mail server you talk to is IPv4-only, they can't reach you. The $3.50 plan adds IPv4, which is why the real entry price for anything public is $3.50, not $2.50.

**Almost no regions.** The $2.50 plan deploys in two US East locations. The $3.50 plan deploys in one. The $5 plan deploys across 31 locations spanning North America, Europe, Asia, South America and Africa. If latency to your users matters, the cheap tiers probably can't serve them.

**Location surcharges.** São Paulo costs more. The $5 plan bills **$7.50/month** there, a 50% premium over the same specs elsewhere. Check the price after you pick a region, not before.

The hourly rates are the part worth exploiting. Every plan is billed hourly as well as monthly, so a $20 plan run for two days costs roughly $1.44, not $20. Use that for migrations, load tests and "will this config survive?" experiments instead of paying for a month you don't need.

## What a cheap VPS actually costs once you add the parts

The plan price covers the instance. It rarely covers everything the instance needs to be useful, and the add-ons are where budget hosting stops being budget:

- **Control panel.** cPanel, Plesk and DirectAdmin usually cost extra. IONOS, for example, charges **$6/month** for Plesk Web Host Edition on top of the server.
- **Backups and snapshots.** Often sold as an add-on rather than bundled. IONOS prices Acronis cloud backup from **$0.065/GB/month**.
- **Extra IPv4 addresses.** One is normally included; additional ones are billed. IONOS charges **$5/month per extra IPv4**.
- **Renewal increases.** Introductory pricing that jumps after the first term. Hostinger's **$4.99/month** runs for the first 24 months only.
- **Managed support.** Unmanaged plans are cheap because you are the support.
- **Migration, security scanning, advanced monitoring, bandwidth overage.** Each one is a line item somewhere.

Vultr's own advantage here is that its plan prices read as ongoing monthly rates rather than first-term teasers, and bandwidth allowances are generous: 1 TB on the $5 plan, 2 TB on the $10 plan, up to 15 TB on the largest. Most small sites use a fraction of that.

The rule that saves the most money: compare the final monthly bill with backups, panel, security and support included, not the number in the headline. A $2 server plus a $6 panel plus backup fees is a $10 server with worse specs.

👉 [See what the $6 High Performance plan includes before you add anything](https://www.vultr.com/pricing/?ref=9738262-9J)

## How much server do you actually need?

These thresholds hold across providers, not just Vultr:

| Resource | What's enough |
| --- | --- |
| **1 vCPU** | Entry level. Fine for a static site, a test box, low-traffic apps. |
| **2 vCPU** | Growing sites and apps, anything running cron jobs and a database at once. |
| **1 GB RAM** | Testing and tiny sites. Will struggle with WordPress plus a panel. |
| **2 GB RAM** | A small WordPress site with plugins. |
| **4 GB+ RAM** | WooCommerce, multiple sites, or a control panel on top. |
| **20–50 GB SSD/NVMe** | Typical for cheap plans. Vultr gives 25 GB at $5, 80 GB at $20. |
| **~1 TB bandwidth/month** | Common baseline. Vultr starts at 0.5 TB and goes up from there. |

A second opinion from the other side of the market: IONOS says 512 MB is enough for a simple website, but puts multiple complex sites or a game server at **8 GB of RAM minimum**. Both numbers describe the same curve. The low end exists, it's just narrower than the marketing implies.

Map that onto real workloads:

- Personal blog or portfolio: 1 GB, and put the savings into backups.
- One WordPress site with WooCommerce: **4 GB**, because PHP, MySQL and a panel competing for 2 GB is how sites fall over during a sale.
- Multiple sites on one box: 4 GB minimum, 2 vCPU, and watch the disk more than the RAM.
- Game server (Minecraft, CS): 4 GB is the practical starting point; 8 GB if mods are involved.
- Dev/test, cron jobs, bots: 1 GB and hourly billing.

## How Vultr compares to the other cheap names

Prices below are the entry points each provider publishes, in the currency they publish them in. None of these are apples-to-apples on specs, so read the notes column.

| Provider | Entry price | What stands out / what to watch |
| --- | --- | --- |
| **IONOS** | from **$2/mo** | 99.99% availability, NVMe, unlimited traffic up to 1 Gbps, data centers in the US, UK, Germany and Spain. Plesk $6/mo, Acronis backup $0.065/GB/mo, extra IPv4 $5/mo. |
| **Vultr** | from **$2.50/mo** | IPv6-only at that price, $5 gets IPv4 and 31 regions. Up to 15 TB bandwidth on large plans. Hourly billing on every tier. |
| **Hetzner Cloud** | **€4.35/mo** | NVMe plus AMD EPYC, regions in Germany, Finland and the US. Priced in euros. |
| **OVHcloud** | ~**$5/mo** | Unlimited traffic up to 500 Mbps and a wide global network. |
| **Netcup** | **€3.35/mo** | 2 vCore, 2 GB RAM, 64 GB SSD at that price. Strong value if you're in Europe. |
| **DigitalOcean** | from **$4/mo** | 512 MiB to 256 GiB range, 1–48 vCPU. No refunds, and its billing flow is more complicated than most. |
| **Hostinger** | **$4.99–$19.99/mo** | That's the first 24 months. No managed hosting, no Windows VPS. |

Where each one wins: Hetzner and Netcup for European traffic and euro billing. OVHcloud when you need a specific country's data center. IONOS when you want a big brand with a $2 entry and don't mind paying separately for panel and backup. DigitalOcean if you're already in its ecosystem and won't need a refund. Vultr when you want the lowest entry point that still includes IPv4, a wide choice of regions, and hourly billing you can actually use to test.

If your project is Windows-based, cross Hostinger and Netcup off the list early; neither sells Windows VPS plans.

## Before you click deploy

Five things to check that the pricing table won't tell you:

1. **Refund or trial terms.** Vultr's plan pages don't advertise a money-back window the way IONOS and Hostinger do (both publish 30 days). Read the terms before you pay, or treat hourly billing as the trial.
2. **Backup and snapshot charges.** Confirm whether automatic backups carry a separate monthly fee, and what a snapshot costs to store.
3. **Whether a control panel is included.** On most budget plans it isn't. If you need cPanel or Plesk, price the license with the server.
4. **Region pricing.** Pick the location first, then confirm the price. São Paulo costs 50% more on the same Vultr specs.
5. **Overages and fair use.** Know what happens when you pass your bandwidth allowance.

## FAQ

**Can a $2.50 VPS run WordPress?**
No. It has 0.5 GB of RAM and no IPv4 address. WordPress with MySQL needs 1 GB as an absolute floor and 2 GB to be comfortable. Budget $10/month for a real WordPress site, or $6 if you're running a static site generator instead.

**1 GB or 2 GB of RAM?**
1 GB for a static site, a proxy, a bot, or a dev box. 2 GB the moment WordPress enters the picture. The jump from $5 to $10 buys you 30 GB more disk and double the bandwidth as well, which is usually worth it before you need it.

**Do I need to know Linux?**
Yes, on this class of hosting. Vultr sells the instance, not the management: you pick the OS image, install the stack, patch it and fix it. If "I don't want to touch a terminal" describes you, a managed plan at a higher price is the honest answer.

**Is 1 TB of bandwidth enough?**
For almost every small site, yes. Text and images for a few thousand visitors a month sit far below 1 TB. Video and large file downloads are the exception, and Vultr's higher tiers go to 2, 3 and 4 TB before you hit the $40 plan.

**Does the $300 credit apply to these plans?**
Vultr's own coupons page lists code **FLY300VULTR** for $300 in promotional credit, restricted to new customers, applicable to select products only, and not combinable with other offers. It's credit you spend on servers, not cash, and the full restrictions live in the terms. There are also $200 and $250 variants and a deposit-match offer up to $100. Apply the code before you deploy, not after.

**Can I start small and resize later?**
Yes, and that's the cheapest path. Start on hourly billing with the smallest plan that boots, watch real CPU and RAM usage for a week, then move to a monthly plan sized from actual numbers rather than guesses.

## Which plan to pick

Blog, portfolio, static site, or a test box: the **$6 High Performance** tier. It beats the $5 Regular plan on storage type and bandwidth for a dollar more, and you'll never notice the difference in the bill.

One WordPress site: **$10** on Regular Performance, or **$12** on High Performance if you want NVMe and the extra terabyte.

WooCommerce, membership sites, or three-plus sites on one box: **$20** for 2 vCPU and 4 GB. This is the tier where a sale-day traffic spike stops being a crisis.

Anything above $40: only if you can name the workload that needs it.

One last thing to confirm at checkout: your region. It changes both latency and, in São Paulo's case, the price.

👉 [Pick a plan and deploy your first Vultr instance](https://www.vultr.com/pricing/?ref=9738262-9J)
