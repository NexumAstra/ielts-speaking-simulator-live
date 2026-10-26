# Speaking assessment rules

## Authority and evidence

The supplied `official/ielts-speaking-band-descriptors.txt` and its PDF are the criterion-level authority. Read the candidate band and adjacent bands before deciding. The PDF notes require the positive features of a level to be satisfied and rating across all parts. The supplied Scores Guide PDF p. 9 identifies the four speaking criteria. The Writing Key Assessment Criteria is not a speaking rubric.

The current public [IELTS scoring page](https://ielts.org/take-a-test/your-results/ielts-scoring-in-detail?authuser=0) confirms equal weighting for the four speaking criteria. Keep Speaking aggregation distinct from the overall IELTS average of Listening, Reading, Writing and Speaking.

For each criterion, build a small evidence record with actual question IDs, verbatim answer excerpts and observable patterns. Look for representative behavior across parts rather than rewarding one rehearsed sentence or penalizing one isolated slip. Explain why the next band is not yet supported. Use integer criterion bands (1–9) corresponding to the published descriptor rows; do not invent official 6.5 descriptor wording. Borderline uncertainty can be explained separately.

Band 0 in the source denotes non-attendance/non-completion. For a simulator's interrupted or unavailable recording, report “incomplete / insufficient evidence”, not an automatic ability band of 0. Distinguish genuinely minimal intelligible language from technical failure.

## Four criteria

| Criterion | Observe | Do not substitute |
|---|---|---|
| Fluency and coherence (FC) | Actual continuity, hesitation/repetition/self-repair patterns, sustained turns, coherent development and natural spoken linking | Speaking fast, excessive connectors, text length, neatly edited transcripts |
| Lexical resource (LR) | Range, precision, appropriacy, collocation, flexible paraphrase, natural idiomatic usage across topics | Counts of rare words, fixed idiom quotas, memorized synonym lists |
| Grammatical range and accuracy (GRA) | Range and flexibility, frequency of accurate sentences, simple/complex structures, effect of errors on communication | Essay punctuation, transcription spelling, long sentences alone |
| Pronunciation (P) | Intelligibility, sound production, chunking, rhythm, stress, intonation and connected speech actually heard | Accent origin, native-accent imitation, transcript correctness, microphone quality |

Band 6/7/8 calibration reminders, subordinate to the full table:

- FC: 6 can sustain speech but coherence may be disrupted; 7 can produce long turns readily with hesitation that does not disrupt coherence; 8 develops topics coherently with most hesitation related to content.
- LR: 6 has adequate resources and generally successful paraphrase; 7 uses resources flexibly, with some less-common/idiomatic language and awareness of collocation; 8 conveys precise meaning with wide, flexible resources despite occasional inaccuracies.
- GRA: 6 mixes forms with limited flexibility, and complex-form errors rarely obstruct meaning; 7 uses simple and complex sentences effectively with frequent error-free sentences; 8 has a wide flexible range and mostly error-free sentences, with occasional non-systematic errors.
- Pronunciation: read the FULL band 6 and 8 feature lists. Band 7 requires all positive features of 6 and some of 8. Band 5 bridges 4 and 6, and band 3 bridges 2 and 4. Do not replace these with made-up independent descriptors.

No separate “content knowledge”, “Task Response” or “Task Achievement” score. Relevance contributes to coherent topic development. Missing one cue-card bullet does not trigger an automatic band cap. A target band, confidence, nationality, school, accent identity or number of sophisticated words cannot determine a score. Do not infer cheating or memorization from polish alone.

## Modality gate

- **Audio accessible**: score all four only when speech evidence is sufficient across all three parts. Use concrete heard pronunciation examples. Provide timestamps only if actually supplied/available; otherwise cite the answer location. Do not invent phoneme errors.
- **Transcript only / dictation**: estimate LR and GRA cautiously from the text. Comment on coherence; FC as a combined criterion is “无法完整评定（缺少实际语流证据）”. P is “无法评定（没有可访问音频）”. No full speaking total. Mark recognition artifacts as uncertain rather than candidate errors.
- **Typed answers**: offer language-practice feedback and provisional LR/GRA evidence only, with the same audio limits. Do not label it a speaking test result.
- **Only one part or very little speech**: give limited practice feedback, not a complete-test score. No minimum word-count penalty; explain what evidence is missing.
- **Audio transferred to a text-only evaluator**: do not inherit an unverifiable pronunciation score from the voice interface. If a prior audio assessor left traceable observations, label them as reported evidence and state that you did not hear them yourself. Ask for accessible audio before claiming an independently checked full score.

## Transparent aggregation for the simulator

Only if the complete test supports all four criteria:

`raw_mean = (FC + LR + GRA + P) / 4`

Display a simulated speaking band using a **conservative lower half-band** at quarter-band midpoints:

`simulated_band = floor(raw_mean * 2) / 2`

Examples: 6,6,6,7 → raw 6.25 → simulated 6.0; 6,6,7,7 → 6.5; 6,7,7,7 → raw 6.75 → simulated 6.5. Always show the raw mean alongside the displayed band and explain the midpoint convention in the written score note.

This is an explicit simulation display convention, not a claim to know the current confidential examiner procedure. The supplied files do not establish midpoint rounding within Speaking. An IELTS-published 2017 research report describes down-rounding within Speaking (printed p. 20, PDF page 21): [Nakatsuhara, Inoue and Taylor](https://ielts.org/cdn/Research/investigation-into-double-marking-methods-nakatsuhara-et-al-2017.pdf). It is historical research, not proof of unchanged current operational rules. Do not import the public overall IELTS `.25/.75` upward-rounding rule into the four Speaking criterion mean. If an authoritative current Speaking-specific rule is supplied later, review and explicitly revise this convention.

If any criterion is unassessable, show no aggregate and never renormalize the remaining criteria into a supposedly complete Speaking result. Every numerical result is an estimated practice assessment, not an official certificate.

## Feedback quality

Use actual evidence: “Part 2 中你说 ‘…’，这个搭配使意思不够准确；可改为 ‘…’。” Explain a pattern and a useful action rather than listing every error. Separate grammatical mistakes from valid variants and transcription mistakes. For pronunciation, distinguish intelligibility from accent and source problems. Limit the main improvement plan to three actions the candidate can practice immediately.

In voice, summarize completion, assessable results, the main strength and priority. Keep the full table, corrections, samples and history in text. Do not announce a precise statistical confidence percentage without a calibrated method.
