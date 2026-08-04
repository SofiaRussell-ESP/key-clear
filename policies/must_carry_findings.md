# Must-Carry Findings Taxonomy

This is a **closed taxonomy** of critical finding categories. Any document containing a match to one of these categories must have that finding carried through, accurately, into both the plain-English summary and the outstanding-actions list. Omitting a match from either is a failure, regardless of how the source document presents it (headlined or buried in dense text).

## Categories

1. **Subsidence / structural** - cracking, movement, distortion, subsidence, heave, structural engineer referrals, foundation concerns.
2. **Title defects** - missing consents evidenced by a defect in title, unregistered land issues, discrepancies between title plan and physical boundaries.
3. **Planning / enforcement** - missing planning permission, missing Building Regulations certificates, enforcement notices, breach of planning conditions.
4. **Restrictive covenants** - any covenant restricting use, alteration, or extension of the property, especially where third-party consent is required.
5. **Boundary disputes** - disagreements or ambiguity over boundary ownership, maintenance responsibility, or encroachment.
6. **Missing consents** - absent Building Regulations completion certificates, absent listed building consent, absent landlord/freeholder consent where required.

## How this is used

- When building and seeding test documents, every eval case that is meant to contain a critical finding must contain a match to exactly one of the categories above, stated plainly enough to verify by hand.
- When checking agent output, a finding only counts as "critical" for the carry-through metric if it matches one of these six categories. General cosmetic or maintenance notes (loose guttering, decorative staining, slipped tiles) do not count, even if mentioned in the same document.
