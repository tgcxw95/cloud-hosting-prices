# cloud hosting providers: real prices compared, hidden fees explained, and how to pick the right tier for your project

Most people searching for cloud hosting providers are really asking two questions: which category do I need, and what will this cost by month twelve rather than month one. Short answers first. Unmanaged cloud servers start at $2.50–$5 per month. Managed cloud hosting runs roughly $8–$35. The hyperscalers — AWS, Google Cloud, Azure — bill by usage with no meaningful floor. Compare brands within the right category and the decision gets much easier; compare across categories and you'll either overpay or end up administering a server you never wanted.

One warning before the numbers: 2026 has not been kind to hosting prices. Memory and SSD costs spiked because AI data centers are absorbing DRAM and flash supply, and at least one well-known provider raised prices twice in three months. Any roundup still quoting last year's numbers is doing arithmetic on fiction.

> **Quick picks**
>
> - **Best value for developers:** Vultr — entry plans from **$2.50/mo** (IPv6-only) or $5/mo with an IPv4 address, across 30+ data centers. 👉 [check Vultr's current plans and prices](https://www.vultr.com/pricing/?ref=7268283)
> - **Cloud power without server admin:** Cloudways — $11/mo, managed, hourly billing, running on a choice of five cloud providers.
> - **Premium managed WordPress:** Kinsta — $35/mo on Google Cloud C2/C3D machines.
> - **Bandwidth-heavy projects:** Akamai Cloud (Linode) — $5/mo, with egress overage at $0.005/GB.
> - **Enterprise and complex apps:** AWS, Google Cloud, Azure — pay as you go, self-managed.

The rest of this article shows where these numbers come from, what the sticker prices leave out, and which plan fits which situation.

## What cloud hosting providers actually sell

The most common buying mistake in this market isn't picking the wrong brand — it's picking the wrong category. Cloud hosting comes in three flavors, and mixing them up is how people end up either overpaying or drowning in a terminal.

- **Unmanaged cloud servers** (Vultr, DigitalOcean, Akamai Cloud, Hetzner, AWS Lightsail): you rent a virtual machine with root access and handle the OS, patches, and web stack yourself. Cheapest per month, most control, all of the responsibility.
- **Managed cloud hosting** (Cloudways, Kinsta, Hostinger Cloud): the provider runs the server stack, caching, security patches, and backups. You manage the website and nothing else.
- **Hyperscale clouds** (AWS, Google Cloud, Microsoft Azure): hundreds of services, fine-grained billing, the steepest learning curve. These three held a combined 63% of the market in Q2 2026 — AWS 28%, Azure 20%, Google Cloud 15%, per Synergy Research Group.

A $5 unmanaged server and a $35 managed plan aren't competitors. One sells infrastructure; the other sells the absence of system administration. Decide the category first, then compare brands inside it.

## Vultr plans and pricing: what you actually get

Vultr is an unmanaged cloud server provider with 30+ data center locations, and its entry pricing is the lowest verified in this comparison: **$2.50/mo on an IPv6-only instance**, $5/mo once you add IPv4. Nobody patches that server for you. That's the trade.

A HostingInfos comparison updated in September 2026 — with prices re-checked on each provider's official pricing page — verified these Vultr plans:

| Plan | Key specs | Price | Billing | Get started |
| --- | --- | --- | --- | --- |
| Cloud Compute (entry, IPv6-only) | Entry plan, IPv6-only | $2.50/mo | Monthly | [See current plans](https://www.vultr.com/pricing/?ref=7268283) |
| Cloud Compute (entry, with IPv4) | Entry plan plus an IPv4 address | $5/mo | Monthly | [See current plans](https://www.vultr.com/pricing/?ref=7268283) |
| High Frequency | 2 GB RAM, 64 GB NVMe | $12/mo | Monthly | [See current plans](https://www.vultr.com/pricing/?ref=7268283) |
| Optimized Cloud | 4 GB RAM, 100 GB NVMe | $28/mo | Monthly | [See current plans](https://www.vultr.com/pricing/?ref=7268283) |

These four rows are a sample rather than the whole catalog — Vultr's pricing page lists the full current range, so 👉 [see Vultr's pricing page for the complete lineup](https://www.vultr.com/pricing/?ref=7268283) before assuming the cheapest listed plan is your only option.

On performance: Hosting-Ranked's 90-day benchmark, published in March 2026, measured Vultr's average time-to-first-byte at 75 ms — 42 ms US-East, 45 ms EU-West, 139 ms APAC — with 99.98% uptime, or 15 minutes of downtime across two incidents in three months. Two honest takeaways from that data. APAC latency was worse for every provider tested, so the region you choose matters more than the logo you choose. And Lightsail and Google Cloud logged perfect uptime in the same window, which tells you the gap between competent providers is smaller than their marketing departments imply.

Who Vultr fits: developers comfortable in a Linux terminal, projects that need geographic spread without enterprise pricing, and anyone who'd rather spend an hour on setup than pay a monthly premium for someone else to do it.

Who should skip it: if "SSH in and apply security patches" sounds like a chore you'll postpone indefinitely, an unmanaged server stops being a bargain and becomes a security liability. The managed tier exists precisely for you.

## Why cloud prices got weird in 2026

Cloud spending is booming, and hardware costs are why your quote changed. Worldwide spending on cloud infrastructure services hit $143.4 billion in Q2 2026, up about 43% year over year — the fastest growth in eight years, again per Synergy Research. Gartner expects public cloud spending to grow another 21.3% this year. AI drives both numbers, and AI also drives the price hikes: AI demand is what's soaking up the world's DRAM and flash supply, and providers are passing memory costs through.

Hetzner is the clearest example. It raised prices on April 1, 2026, then again on June 15, 2026. The entry CX23 plan (2 vCPU, 4 GB RAM) went from €3.99 to €5.49 a month; the AMD-based CPX22 jumped from €7.99 to €19.49. The detail most roundups miss: the new prices apply to new orders and to rescales of existing servers. Planning to resize your Hetzner instance? The resize itself can trigger the new rate.

One more number worth knowing before you pick any plan: Flexera's 2026 State of the Cloud report puts estimated wasted cloud spend at 29% — the first increase after five years of decline. Right-sizing your server matters as much as picking the right provider, and it's the reason "just get a bigger plan to be safe" is expensive advice.

## Cloud hosting providers compared (September 2026 pricing)

Here's the head-to-head on verified September 2026 prices, management model, and the detail that actually separates each provider:

| Provider | Best for | Starting price | Managed? | Standout detail |
| --- | --- | --- | --- | --- |
| Vultr | Global reach on a budget | $2.50/mo (IPv6-only), $5/mo with IPv4 | No | 30+ data center locations |
| DigitalOcean | Developers and startups | $4/mo | No | Per-second billing since Jan 1, 2026 |
| Akamai Cloud (Linode) | Bandwidth-heavy sites | $5/mo | No | Egress overage at $0.005/GB |
| Hetzner Cloud | Cheapest RAM in Europe | €5.49/mo plus IPv4 | No | 20 TB traffic in EU regions; limited stock |
| AWS Lightsail | Easy entry into the AWS ecosystem | $3.50/mo (IPv6), $5/mo with IPv4 | No | 3 months free on select bundles |
| Cloudways | Managed cloud for SMBs and agencies | $11/mo | Yes | Choice of 5 underlying clouds, hourly billing |
| Hostinger Cloud | Beginners who want cloud power | $7.99/mo (48-month term) | Yes | Renews at $25.99/mo |
| Kinsta | Premium managed WordPress | $35/mo | Yes | Google Cloud C2/C3D machines |
| AWS, Google Cloud, Azure | Enterprises and complex apps | Pay as you go | Self-managed | 63% combined market share |

A few notes on that table. Hetzner has the strongest price-to-RAM ratio in Europe and a generous 20 TB traffic allowance in its EU regions, but stock is limited and the traffic perk is region-focused. Vultr's edge is breadth — 30+ locations means you can put compute near users in markets Hetzner doesn't cover. Lightsail is the gentlest on-ramp to AWS, and three free months on select bundles is a genuine offset if your project has a defined lifespan.

## The costs that never make the headline price

Sticker prices hide three things, and each one can rewrite your budget.

**Egress fees.** Data you push out of a cloud server is billed separately from the plan, and heavy-traffic sites can watch that line item rival the server itself. This is why bandwidth-heavy projects keep getting pointed at Akamai Cloud: its $0.005/GB overage is the rate everything else gets measured against. If your project serves large files or video, price the bandwidth before you price the plan.

**Renewal jumps.** Promotional pricing resets, sometimes brutally. Hostinger Cloud costs $7.99/mo on a 48-month term and renews at $25.99/mo — more than triple. Bluehost starts at $2.09/mo and renews at $4.68. DreamHost starts at $2.89/mo and renews at $10.99. None of this is a scam; all of it changes the math. Always price the 24-month total, not month one.

**Repricing on change.** The Hetzner case above is worth treating as a general rule: before committing anywhere, check whether the provider's current pricing applies to rescales and upgrades, not just new orders.

And if anything about your plan is usage-based, set billing alerts on day one. A traffic spike is good news until the invoice arrives.

## How to choose, based on what you're actually hosting

Match the plan to the job rather than to the review score:

- **Learning Linux or running a hobby project:** take the cheapest unmanaged plan and stop there — Vultr's $2.50 IPv6-only instance or Lightsail's $3.50 IPv6 plan. Move to the $5 IPv4 version when real visitors show up.
- **A production site, and you're technical:** the mid tiers of Vultr, DigitalOcean, and Akamai Cloud finished within a few milliseconds of each other in the benchmark above. Your region choice will move latency more than your brand choice will.
- **WordPress without server skills:** Cloudways at $11/mo is the middle ground — managed, hourly billing, five underlying clouds to pick from. Hostinger Cloud at $7.99 is the budget route if you accept the renewal jump noted above. Kinsta at $35/mo is the premium route, and it tied for the best average TTFB (71 ms, alongside Cloudways) in that benchmark.
- **Serving serious bandwidth:** run the egress math first. Akamai's $0.005/GB is the number to beat, and Hetzner's 20 TB EU allowance covers a lot of media serving if your audience is European.
- **Enterprise workloads, compliance, complex architecture:** the hyperscalers. Self-managed and usage-billed, they're also the tier where 76% of large enterprises now spend over $5 million a month on cloud services.

If that first profile fits — you want a cheap, capable server and you're willing to admin it — 👉 [check Vultr's entry plans and current pricing](https://www.vultr.com/pricing/?ref=7268283) and take the smallest plan that covers the software you want to run.

## Frequently asked questions

### How much do cloud hosting providers cost per month?

Entry-level unmanaged plans run $2.50–$5 per month, managed cloud sits between $8 and $35, and hyperscalers bill by usage with no fixed floor. In every tier, check two extra numbers before committing: the renewal price and the egress rate.

### What's the catch with IPv6-only plans?

The catch is reachability; the reward is price. Vultr charges $2.50/mo instead of $5 for the same instance without IPv4, and Lightsail follows the same pattern at $3.50 versus $5. An IPv6-only server isn't directly reachable from IPv4-only visitors, so treat it as a learning and lab option unless you know your audience can reach it.

### Is Vultr a good choice for beginners?

Only if "beginner" means beginner at hosting prices rather than at server administration. Vultr is unmanaged: root access, your patches, your problem. If you want cloud-level performance without a command line, look at the managed tier instead — Cloudways or Hostinger Cloud at the accessible end, Kinsta at the premium end.

### Why do price lists for the same provider differ between websites?

Three reasons. Prices genuinely moved this year — Hetzner adjusted twice within three months. Comparison sites quote different baseline plans. And the IPv4/IPv6 split creates a $2.50 gap on what is otherwise the same Vultr instance. Check the date and the plan name before trusting any table, including the ones in this article.

## Before you click buy

Four things to confirm, in order:

1. The current price at checkout. This year has already shown that list prices can move mid-year, and a rescale can pull your instance onto the new rate.
2. The region nearest your users. In the benchmark above, APAC latency was worse for every provider tested — region selection is the cheapest performance win available.
3. IPv4 versus IPv6-only, decided before ordering. It changes your entry price by half.
4. Billing alerts, if anything about your plan is usage-based.

If you've read this far, you already know which category you're in. For developers who want wide geographic coverage at entry-level pricing, Vultr is the first name on the shortlist — 👉 [check Vultr's current plans and prices](https://www.vultr.com/pricing/?ref=7268283) and confirm the numbers while they're current.
