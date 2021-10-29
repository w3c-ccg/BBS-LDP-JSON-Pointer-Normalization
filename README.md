# BBS-LDP-JSON-Pointer-Normalization
This proposal describes a BBS signature suite for Linked Data Proofs using JSON Pointer Normalization to generate verifiable data.

## Include Link to Abstract or Draft 

[POC Document](https://github.com/trinsic-id/json-bbs-signatures/blob/main/ldp-bbs-jpn.md)

## List Owners

Tomislav Markovski @tmarkovski (Trinsic)
Jakob Povšič @jkbpvsc (GlobaliD)

## Work Item Questions

1. Explain what you are trying to do using no jargon or acronyms.

This proposal describes a BBS signature suite for Linked Data Proofs using [JSON Pointer Normalization](https://trinsic-id.github.io/json-ptr-n11n-spec/) to generate verifiable data.
The main goal of this signature suite is to define additional BBS signature scheme that utilize simpler algorithms compared to existing ones. This is useful in situations where JSON-LD processors or suites are unavailable.

2. How is it done today, and what are the limits of the current practice?

 Existing [BBS+ Signatures 2020](https://w3c-ccg.github.io/ldp-bbs2020/) scheme uses JSON-LD processors and data canonicalization using URDNA2015 in contrast to this suite which uses simpler normalization algorithm based on JSON Pointer document flattening. This normalization algorithm can utilize selective disclosure and ZKP features defines in the BBS spec.

3. What is new in your approach and why do you think it will be successful?

The core principal in the proposed approach is the use of a simple algorithms for signature generation. It uses normalization algorithm based on JSON Pointer addressing for creating deterministic verifiable object state.

4. How are you involving participants from multiple skill sets and global locations in this work item? (Skill sets: technical, design, product, marketing, anthropological, and UX. Global locations: the Americas, APAC, Europe, Middle East.)

We'd like to invite participants from different backgrounds and skillsets to contribute and ideate on this approach. We believe this community is best suited to expand the use of BBS signatures more broadly in the context of verifiable data.

5. What actions are you taking to make this work item accessible to a non-technical audience?

We've written a draft document that can serve as a starting point to understand the concept for non-technical audience. We'd like this effort to be a point of discussion for the viability of this approach at different levels. The opportunities with using BBS more broadly impact product designs and business decisions more broadly, and we're hoping all of these will be discussed as part of this work item development.
