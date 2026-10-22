# HTML Audit Report(Part A)

## 1. Tagline Used as a Heading

**Defect:** The tagline “Quality You Can Trust!” was marked as an `<h2>`.

**How I proved it:** The heading outline shows `<h1>` for the shop name, followed by `<h2>` for the tagline. The tagline is a slogan, not a section heading.

**Kind:** 2

**How I fixed it:** Changed the tagline to a paragraph.

## 2. Vague Image Alternative Text

**Defect:** The image has unclear alternative text.

**How I proved it:** The HTML contains `alt="image"`, which does not describe the image's content.

**Kind:** 2

**How I fixed it:** Added meaningful alternative text describing the actual image.

## 3. Fake Bullet List

**Defect:** The services are not marked up as a proper HTML list.

**How I proved it:** The code uses `&bull;` and `<br>` inside a paragraph instead of proper list elements.

**Kind:** 2

**How I fixed it:** Replaced the paragraph with `<ul>` and `<li>` elements.

## 4. Unsupported Business Claims

**Defect:** The page contains unverified claims about the shop's history, customers, and awards.

**How I proved it:** The page says the shop was established in 1985, has over 2,000 satisfied customers, and is award-winning. No supporting evidence was supplied.

**Kind:** 3

**How I fixed it:** Removed the claims or requested confirmation from the owner.

## 5. Unverified Deposit Policy

**Defect:** The deposit and refund policy has not been verified.

**How I proved it:** The page states that a 50% deposit is required and is non-refundable, but the supplied information does not confirm this policy.

**Kind:** 3

**How I fixed it:** Requested confirmation from the owner before publishing the policy.

## 6. Unconfirmed Currency

**Defect:** The prices use a dollar symbol without confirming the currency.

**How I proved it:** The pricing section shows `$250.00` for a custom suit and `$20.00` for alterations.

**Kind:** 3

**How I fixed it:** Confirmed the shop's currency and updated the prices accordingly.

## 7. Unverified Contact Number

**Defect:** The contact number has not been verified.

**How I proved it:** The page displays `(555) 123-4567`, which resembles a US-style example number.

**Kind:** 3

**How I fixed it:** Requested a valid contact number from the shop owner.

## Conclusion

This audit taught me that AI-generated HTML can look correct while still containing accessibility, semantic, and factual problems. An HTML validator can detect some technical errors, but it cannot verify every business claim or local detail. Human judgment and reliable evidence are necessary to identify and correct these problems.

(part B)

1. Which of the eight defects did today's model avoid?
The model corrected the tagline heading, improved the image's alternative text, created a proper HTML list, removed unsupported business claims, avoided unverified deposit policies, addressed the currency, removed unverified contact details, and avoided inventing working hours.
2. Which ones did it repeat?
The model still could not confirm the actual business details, including prices, opening hours, the busiest trading day, deposit policy, and contact information. The image description also needs to be checked against the actual image.
3. For each one it repeated, why could no improvement to the model have prevented it?
The model cannot know facts that the shop owner has not provided. Even an improved model would need reliable evidence to confirm the actual prices, working hours, trading day, and business policies. Human verification is necessary to avoid inventing information.

(PART C)

1. Constraint added: State the confirmed currency and actual location of the shop.
Defect removed: Missing currency and location information.
Kind: 1.

2. Constraint added: State the actual working week, including the day that matters most for trade.
Defect removed: Incomplete or unverified trading schedule.
Kind: 1.

3. Constraint added: Use headings to establish a logical document outline rather than choosing heading levels based on their visual size.
Defect removed: Incorrect or inconsistent heading hierarchy.
Kind: 2.

4. Constraint added: Mark important warnings semantically as important, rather than relying on bold text alone.
Defect removed: Deposit warning presented without sufficient semantic emphasis.
Kind: 2.

5. Constraint added: Do not invent, assume, or include any business information that was not provided.
Defect removed: Unsupported claims and potentially misleading business information.
Kind: 3. 



answer in two sentences

Some defects, such as missing currency, location, and the most important trading day, survived the well-written prompt because the original information did not supply those facts. No wording could reliably establish those unknown facts without additional evidence, because a prompt can guide how information is presented but cannot guarantee the truth of information that was never provided.



(PART D)
