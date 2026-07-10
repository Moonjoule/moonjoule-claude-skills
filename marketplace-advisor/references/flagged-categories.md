# Flagged Categories

These item categories require a graceful exit from the standard Marketplace Report
format. For each, explain to the user _why_ the skill's framework isn't the right
tool, then offer what you can — usually an open-ended conversation rather than a
structured report.

The key principle: a structured report on a flagged-category item could give the
user false confidence. Better to be honest about the limits of this skill's
framework than to produce authoritative-looking output that misses the things
that actually matter.

---

## Vehicles (cars, motorcycles, RVs)

**Why flagged:** Vehicle purchases involve a level of legal, mechanical, and
financial complexity that a Marketplace Report format actively misrepresents.
The most important signals — frame damage, odometer fraud, title washing,
accident history, latent mechanical faults — are invisible to visual inspection
and to any amount of research a non-mechanic can do remotely. A report that
assigns a Deal Rating and lists Red Flags creates the impression of due diligence
where the actual due diligence hasn't happened yet.

Key dimensions the report format can't adequately cover:

- VIN history (write-offs, stolen vehicle flags, odometer discrepancies)
- Pre-purchase mechanical inspection (requires a trusted independent mechanic)
- Title and lien status (varies significantly by province/state)
- Insurance implications of vehicle history
- Platform-specific dynamics (Kijiji Autos, AutoTrader, and CarGurus operate
  differently from general Marketplace)
- Lemon law protections, which vary by jurisdiction and often don't apply to
  private sales

**What to say:**

> "Vehicles are a category where I'd do you a disservice with a standard
> Marketplace Report — the things that actually determine whether a used car
> is a good buy (VIN history, mechanical condition, title status) require tools
> and access I can't replicate in a report format. What I _can_ do is help you
> think through this in open-ended mode: what to research, what questions to
> ask, what a pre-purchase inspection should cover, and what red flags look like
> in seller behaviour. Want to do that instead?"

**What you can still offer:** VIN check services to use (Carfax, ICBC in BC,
Service Ontario), what to look for in seller behaviour, how to find and brief
an independent mechanic, platform-specific advice, negotiation framing once
they have inspection results.

**Future skill:** A `/vehicle-advisor` companion skill is planned.

---

## Real Estate

**Why flagged:** Real estate listings occasionally appear on Marketplace and
Kijiji, ranging from FSBO (for sale by owner) listings to rent-to-own schemes
to outright scams (phantom rentals, deed fraud, title scams). The stakes are
categorically higher than any other item on this list — a structured report
could provide false confidence on what is, in almost all jurisdictions, a
legally complex transaction that requires professional representation.

Key dimensions the report format can't adequately cover:

- Title search and lien status (requires a real estate lawyer or notary)
- Property condition (requires a licensed home inspector)
- Zoning, easements, and encumbrances
- FSBO transactions have no mandated disclosure requirements in many jurisdictions
- Rent-to-own arrangements are frequently predatory and poorly regulated
- Marketplace real estate listings skew heavily toward scams (phantom rentals,
  fake landlords, wire transfer fraud) — the scam density is far higher than
  in other categories

**What to say:**

> "Real estate is well outside what this skill's framework is designed for —
> the stakes are high enough that a structured report format could give you
> false confidence on something that genuinely needs a real estate lawyer and
> a licensed home inspector. If you're seeing a listing that looks suspicious,
> I can help you identify red flags in open-ended mode. If you're seriously
> considering a purchase, the most important thing I can tell you is: get
> independent legal representation before signing anything."

**What you can still offer:** Scam pattern identification for suspicious
listings, general questions to ask, explanation of why certain deal structures
(rent-to-own, seller financing) carry elevated risk.

---

## Vintage and Collectible Instruments

**Why flagged:** The skill's core Age Risk Assessment logic — older items carry
higher risk — inverts for vintage instruments with collectible value. A 1965
Fender Stratocaster is not subject to age risk; its age _is_ the value. Applying
a standard report framework here produces absurd results: flagging high risk on
an item whose age is precisely what makes it desirable and valuable.

Additionally, authentication of vintage instruments requires in-person expert
assessment. Counterfeit vintage guitars, fake provenance, refinished bodies
presented as original — these require someone who knows what to look for in
person, not a web-researched report.

This applies to: guitars, basses, amplifiers, keyboards, and other instruments
from the pre-CNC, pre-mass-production era (roughly pre-1980 for most categories)
where individual unit variation and provenance matter significantly.

**Note:** Modern used gear (a 2019 Fender Player Stratocaster, a recent-model
digital piano, a current-production amp) fits fine within the standard skill.
The flagging applies to items where collectibility and age-as-value are in play.

**What to say:**

> "Vintage instruments are a category where my standard framework breaks down —
> the age risk logic I use for appliances and electronics inverts here, because
> the age is part of the value. Authentication also requires someone who can
> inspect the instrument in person; photos and listings can't capture what
> matters. I can still help you think through this, but I'd frame it differently:
> what questions to ask, what the known forgery and misrepresentation patterns
> are for this specific instrument, and what an in-person inspection should cover.
> Want to do that?"

**What you can still offer:** Known forgery patterns for the specific instrument,
what provenance documentation should exist, where to find expert appraisers,
what fair market value looks like for authenticated examples.

---

## Jewellery and Watches

**Why flagged:** Authentication is the central question for anything of
significant value in this category, and authentication cannot be done remotely.
Gold hallmarks can be faked, diamonds can be cubic zirconia, "vintage Rolex"
listings are a well-documented fraud category. A report that assigns a Deal Rating
based on the seller's description and photos actively misleads the buyer about
what due diligence is actually required.

For low-value costume jewellery or fashion watches, the standard skill may be
appropriate — the stakes don't justify specialist intervention. The flag applies
when the listing price or claimed value suggests the authentication question matters.

**What to say:**

> "For jewellery and watches at this price point, the most important thing a
> Marketplace Report can tell you is what it _can't_ verify — and the honest
> answer is that authentication requires in-person assessment by a qualified
> appraiser or gemologist. What I can do is walk you through the known fraud
> patterns for this category, what a legitimate seller's listing typically looks
> like versus a suspicious one, and what you'd need to see before paying. Is
> that useful?"

**What you can still offer:** Common fraud patterns (hallmark fraud, replica
watch tells, synthetic stone presentation), what documentation a legitimate
seller should have, how to find a certified appraiser, what to look for in
seller behaviour.

---

## Boats and Personal Watercraft

**Why flagged:** Similar to vehicles in complexity, but with additional layers:
hull integrity assessment requires out-of-water inspection, marine engines have
specialized failure modes, registration and title vary significantly by province
and country, and freshwater vs. saltwater history matters enormously for
corrosion. A standard report format creates false confidence in a category where
the hidden defects (osmotic blistering, stringers, transom rot) are literally
invisible without haul-out and inspection.

**What to say:**

> "Boats have enough category-specific complexity — hull integrity, engine
> condition, freshwater/saltwater history, registration — that my standard
> report format would give you false confidence on what actually matters.
> Think of it like vehicles: a pre-purchase survey by a qualified marine
> surveyor is the equivalent of a mechanic's inspection, and it's not optional
> for anything worth significant money. I can help you think through questions
> to ask, what seller behaviour flags to watch for, and what a marine survey
> should cover. Want to do that?"

---

## Firearms

**Why flagged:** The legal framework for private firearms sales varies so
significantly by country, province, and state that any general advice creates
genuine risk of legal error. What is legal in Alberta may not be in Quebec;
what is legal in one US state may be a federal crime in the context of an
interstate transaction. This is not a category where a generalised "buyer's
guide" approach is appropriate.

**What to say:**

> "Firearms sales involve jurisdiction-specific legal requirements that vary
> enough that I'd rather not give you a generalised buying guide. The most
> useful thing I can point you to is [jurisdiction-appropriate resource] — the
> rules around private sales, transfer requirements, and registration differ
> significantly even within Canada or the US. If you have specific questions
> about the process in your jurisdiction, I'm happy to try to help."

**What you can still offer:** Point toward jurisdiction-specific regulatory
resources. Do not provide generalised advice about firearms transactions.
