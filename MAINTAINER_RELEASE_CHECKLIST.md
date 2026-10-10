# SADAR README: checks before public release

These notes are separate from the public-facing `README.md` to avoid silently inventing information missing from the uploaded manuscript.

- [ ] Verify the full author list, publication status, venue, year, and DOI/URL. Do not present an AAAI-formatted submission as an accepted AAAI paper without evidence.
- [ ] Replace the `README.md` availability notice with verified dataset and code links and instructions once those files are present.
- [ ] Confirm whether the collection platform / app-store terms allow redistribution of raw review text. Establish annotation and code licensing separately where necessary.
- [ ] Add exact collection dates, five-app sample sizes, annotation file schemas, preprocessing and evaluation splits (if any), and language/encoding instructions.
- [ ] Resolve LLaMA nomenclature: the quantitative table says `LLaMA3.2-3B` while an experiment paragraph says `LLaMA3-8B`. Give the exact checkpoint/tag used.
- [ ] Resolve model counting: the study describes 10 compared models; the quantitative table reports 9. Mixtral-8x7B was excluded due to unreliable instruction following. Document its outputs and exclusion rationale.
- [ ] Archive the literal prompts used in experiments. An appendix prompt previously listed `-1, 0, 1` polarity values, whereas the dataset text uses the binary `0, 1` scheme. Document the actual prompt and any conversion/mapping, without retroactively modifying experimental materials.
- [ ] Verify that the reported `1,751` and `1,257` dataset counts refer to what the table implies. Neutral examples are merged into the dataset's non-positive `0` label.
- [ ] Document the relationship of the 23-level source taxonomy to the 24-category final SADAR inventory and establish canonical labels for `Language/Multilinguality`, `Multi-function/Usage`, and `Consumption/Electronic consumption`.
- [ ] Provide actual dependency/install/inference/evaluation commands and test them from a clean checkout before adding them to the README.
- [ ] Document precision/recall/F1 matching rules and text normalization, especially for partial versus exact ACOS matches and invalid/empty model output.
- [ ] Replace the BibTeX template with the verified citation.
- [ ] Ensure distributed results / figures match Table 2 and Appendix F; check the 24 bar-chart counts against the final annotation files.
