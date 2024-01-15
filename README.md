# Motivation
We live in a world where online marketplaces are drowned out by unaccountable companies with [intentionally gibberish names](https://www.youtube.com/watch?v=4UrqlMfwUC4) flooding the listings with products that barely work, if at all, competing not by the way of products or services that are proudly stood behind, but through fake reviews and other deceptive business practices. Even forsaking particular marketplaces like Amazon and eBay, search engines and product reviewers sell out to the highest bidder, and big retailers are happy to offer anything just shy of an outright scam to bring prices as low as possible or errode ownership as much as possible to sip that sweet, sweet recurring revenue. It can take tremendous effort to sift through all of the consumerism-induced noise to find reliable products / services that last and are sold -- not on lease or a subscription.

This repository aims to crowdsource the discovery of these functioning products & services that respect the consumer. Maybe one day it will be large enough to compete with the likes of Amazon!

# Key Tenants

## Quality
All listed products must meet at least this metric. If they meet others but fail this one, they cannot be listed.

Quality is the hardest metric to measure. It is both subjective, and can take years to accurately determine. It would be impossible to guarantee that a product released this year would live up to the manufacturer-promised lifetime of 10 years without testing many copies of the product over the course of 10 years. This is even harder for products with internal components that can't be easily observed and software that can only be validated through exhaustive testing. To compensate, we look at things we can measure or easily test that have a high correlation with product quality.

### General
- Warranties are not considered as a substitute for product quality since companies may offer lifetime warranties for terrible products with the intention of them being lifetime in name only & weasling their way out, or only offer 1-2 years on a product that generally lasts for 10
- If it looks like the manufacturer took any shortcuts, fail
- If there are a non-negligible amount of product reviews on other platforms that complain about reliability under reasonable circumstances, fail
- They must have a company website/email outside of Amazon and a physical address

### Hardware
If the product is made of multiple components, it must be torn down

#### Materials
- Deceptive materials (e.g. plastic masquerading as chrome metal) fail
- Nonpremium faux materials fail
- Fibreboard, plywood, and scrap wood (e.g. pallets) fail
- Plastic moving components (e.g. plastic gear) fail unless as a non-cost design consideration (e.g. drone components have to be as light as possible)
- If it feels obviously flimsy for its intended purpose, it fails


#### Load
- If documented tolerances are not at least 2x a reasonable load (e.g. 250 lbs is 90% percentile US mail weight and a reasonably expected load), it fails
- If documented tolerances don't hold up under nonstandard but reasonable load (e.g. doing swings on a standing pull up bar makes it rock back and forth), it fails
- Try to use the product incorrectly (e.g. drill through metal rather than wood) and it breaks or degrades in an unreasonable way (e.g. the drill breaks and not the bit), it fails
- If the product breaks or degrades under heavy but normal use, it fails
- If furniture cannot support an adult jumping up and down on it, it fails
-  

### Software / Firmware
- If it should be able to be used without a mobile app but requires one, fail
- 

## Reputable Origins
A product or service's country of origin can have significant impact on a consumer's ability to trust & hold accountable a company. Even if a product is designed by a reputable company, products manufactured in nonreputable countries with lax or nonexistent consumer / business protection regulations may:
- Flagrantly lie and break guarantees the designing company makes to consumers
- Use knock-off parts without the knowledge of the designer
- Use unsafe materials / manufacturing processes that are banned in reputable countries
- Not be able to be held accountable by the law if they lie to designers/consumers and/or hurt consumers
- Utilize slave or sweatshop labor

Therefore, it is impossible to completely trust that the bar of relevant tenants are actually met if the origin of a product is not reputable. Unfortunately, even the most reputable of products are outsourced to nonreputable countries for manufacturing these days, so completely eliminating these products would be impractical. Instead, since country of origin does not affect metrics like repairability and ownership, a reputable origin is only a hard requirement in certain cases (noted in relevant tenants below), and this metric is purely informational otherwise. Regardless of whether the country of origin is reputable, all products must have a known country(ies) of origin set in their metadata, as well as the founding date of the company.

The following countries are considered reputable at this point in time:
- United States
- Canada
- European Economic Area
- United Kingdom
- Switzerland
- Australia
- New Zealand

## Repairability
1. Fully and practically user-servicable, not restricted to "authorized" repair centers
2. Specific parts available (i.e. screen cable can be bought on its own, and not an entire screen assembly) at reasonable prices and reasonable availability
4. Manufacturer does not prevent or combat others selling competing replacement parts 
5. Any software needed to do repairs is open source and not reliant on cloud servers from the seller
6. Manuals and schematics available

## Ownership
1. Fully meets the "Repairability" criteria
2. Fully functional on LAN connection, if there is network connectivity. Does not force you to connect to the Internet
3. No remote killswitches or backdoors
4. No lockouts/subscriptions for hardware you already have physical access to (e.g. heated seats)
5. Subscriptions only allowed for services that are a recurring cost to the provider (otherwise must be one-time purchase) and must be optional or replaceable with a competitor's service
6. Does not violate Magnuson Moss Waranty act 

## Sustainability
To quote [Framework](https://frame.work/sustainability)
> We are not sustainable
> 
> And neither is any other device maker. This industry is full of “feel good” messaging, but generates 50 million metric tons of e-waste each year. We believe the best way to reduce environmental impact is to create products that last longer, meaning fewer new ones need to be made.

Even if an Amish woodworker drops a 100% natural wood carving that was manufactured with sweat rather than machinery powered by coal-fueled electricity off at the post office, which then gets packaged in a 100% paper box with 100% paper filling, and is then delivered on the last leg of its journey to your door in an electric-powered delivery van, the plane or semi that moved the package from Pennsylvania to California burned fossil fuels, and that paper box/filling, EV delivery van, and their raw materials were likely manufactured & obtained through non-sustainable means. The post workers who received the package likely drove to work in gas-powered vehicles, and the post office is likely powered by nonsustainable electricity.

Complete sustainability is a myth, and as such this respository focuses purely on factors within the product seller/designers' direct control and lack of deceptive greenwashing. More specifically:

**Design:**
1. Any disposable materials must be as minimal as possible. A mop with compostable, disposable pads is not sustainable and should have washable pads instead.
2. Any nondisposable materials must meet the Repairability criteria above

**Materials:**
1. Packaging & disposable materials must be consumer-compostable (i.e. compostable in the consumer's backyard and do not require an industrial facility) or sustainably recyclable
    - This includes labels & tapes on the packaging, which rules out anything from Amazon warehouses at this point in time
    - Sustainably recyclable means that it is profitable to recycle, that it is universally accepted in curbside recycling, and requires <= the amount of energy to re-manufacture (i.e. energy to pick up your bin + sort at the recycling facility + ship to manufacturer + manufacture into another product <= energy to mine raw materials + distribute to the manufacturer + manufacture into a product). This currently entails only metal, glass, and unsoiled paper.
    - Food cans and laminated paper do not meet this criteria even though they are recycleable because of their coatings
    - Products that are _technically_ sustainable under this criteria but not _practically_ (e.g. requires extensive cleaning or handling) fail the criteria
2. Nondisposable materials that aren't single use must either be compostable/recyclable or inert materials (pottery, stone, or silicone)
    - This excludes all electronics
3. Consumables like toothbrushes or razors that are designed to be regularly replaced are considered disposable materials

**Marketing:**
1. Any advertised biodegredation or composting must be home-grade (e.g. OK Compost Home and not OK Compost Industrial). The term "biobased" is banned.
2. If a product is advertised as compostable/recyclable, then the whole product must be compostable under this criteria, even if it is not disposable. 

## Verifiable
Should be verifiable by others, so local shops that do not ship throughout at least all of the contiguous US or EU are prohibited. Expensive luxury products (e.g. $10,000 watch) are not practically verifiable by others and are also prohibited.
