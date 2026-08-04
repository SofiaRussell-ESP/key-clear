# Escalation Policy

Escalate to the human buyer, stating the reason, when any of the following apply.

## Low confidence
- The document is illegible, garbled, or otherwise cannot be reliably translated.
- It is unclear whether a deadline is actually present in the text.

## Missing data
- The document is corrupted or inaccessible.
- Default rule: if a requirement or action is described as needing to happen before a milestone (completion, exchange) and the document does not give an exact date or timeframe, treat this as a missing deadline - flag DEADLINE as "Missing - deadline implied but no date given" and escalate. Do not borrow a target date from the case profile to resolve this; a document's deadline only counts as known if that document itself states a specific date or timeframe.
- The ONLY exception: the document contains an explicit phrase telling the buyer their own timing is flexible - specifically "when you get a moment," "at your convenience," "no rush," "no immediate deadline," or clearly equivalent wording, directly attached to what the buyer is being asked to do. When that exact kind of phrase is present, flag DEADLINE as "None stated" instead and do not escalate for missing data.
- This exception requires that literal phrase. It does NOT apply just because urgent language is absent, or because the solicitor describes their own pending check with a third party (e.g. "we are checking with your lender and will confirm") - that is still a real requirement pending an unstated date, not an explicit grant of flexibility to the buyer.
- A specific fact, figure, or finding the buyer needs is described as being in an attachment, and that content never actually appears anywhere in the document provided (for example, a letter that says "see attached plan for boundary details" with no further detail given anywhere).
- This does NOT include a routine reference to an enclosed form or document where the letter already fully explains what is needed and by when (e.g. "please countersign the enclosed form and return it by [date]"). That is a normal action item, not missing data - the buyer clearly knows what to do even without seeing the form itself.

## Legal / high-impact language
- The document uses urgent, threatening, or unusual-pressure language (e.g. "act now," "failure to respond may result in...").
- The document reveals an active dispute, an enforcement notice already issued, or demands an immediate legal response beyond a routine specialist referral.
- Standard solicitor correspondence that simply uses normal conveyancing terminology ("exchange of contracts," "completion," "enquiries") to request a routine document or signature is NOT legal/high-impact language on its own.
- A must-carry finding on its own (per must_carry_findings.md - e.g. a structural survey flag, a restrictive covenant, a title or planning issue) is NOT legal/high-impact language requiring escalation. Surface it clearly in CRITICAL_FINDINGS, flag ACTION_REQUIRED as Yes, and draft a response recommending the buyer discuss it with their solicitor or arrange the relevant next step (e.g. a structural engineer's inspection, indemnity insurance). Do not refuse to draft a response just because a must-carry finding was found - escalate only if it is also paired with urgent/threatening language or another trigger in this policy.

## Out-of-policy request
- The buyer or a document asks the agent to judge whether a search result, survey finding, or contract term is "safe" or "fine to accept."
- The buyer or a document asks the agent to suggest a counter-offer, a price adjustment, or any negotiation position.
- In these cases: hard refusal. State that this judgment sits with the buyer and their solicitor. Do not draft any response that takes a position on price or acceptance.

## High stakes
- Funds are due today or within 24 hours.
- The buyer must act immediately to avoid missing exchange of contracts or completion itself (same-day instructions, or a deadline of less than 24 hours).
- This does NOT include a routine action item that simply has exchange or completion as its eventual target date. A normal request with several days' notice ("send us X by [date] so we stay on track for exchange") is routine, not high stakes.

## Suspected fraud
- Payment or account details in a message differ from the previously recorded solicitor details on file (see case_profile.csv), even slightly.
- Urgency language is paired with a request to change payment method or destination account.
- In these cases: never draft a response of any kind. Escalate directly to the buyer with an explicit warning to verify the request via an independent, known channel (e.g. a phone number already on file) before taking any action. Never treat this as a routine action item.
