# Mobile and live voice

Checked against official OpenAI documentation on 2026-10-25:

- [Plugins](https://learn.chatgpt.com/docs/plugins): account-available plugins can be used in mobile Chat and Work; desktop-only plugins are an exception.
- [Build skills](https://learn.chatgpt.com/docs/build-skills): plugin-bundled skills can be available on mobile.
- [ChatGPT Voice](https://learn.chatgpt.com/docs/features/voice): documents live conversation, rollout/workspace dependencies, and an iOS path through a paired desktop host.

These pages do NOT verify this specific plugin's simultaneous skill loading, reference retrieval, audio access and timing behavior in both iOS and Android live voice. Do not promise verified Android or iOS end-to-end support solely because installation succeeded. There is no plugin manifest switch that enables unavailable host voice features.

## Intended phone workflow (iOS and Android)

1. Open the saved plugin in the same account/workspace and enable/install it if prompted. Start a new chat and select the plugin by its exact name.
2. Upload question files in the text interface before starting voice, if desired. Ask the plugin to load the question plan and rubric without revealing the future questions.
3. If that chat offers live voice and preserves the plugin context, start voice. Say “开始完整雅思口语模拟考试”. The examiner asks one English question at a time.
4. Use “Pause”, “Resume”, “Repeat”, “Ready” and “Finished” as needed. A one-minute phone timer can handle Part 2 preparation when exact host timing is unavailable.
5. At the end, hear a brief result and open the written report for the four-criterion evidence, sample answers and question history.

If the current mobile voice surface cannot load plugin skills or files, do not claim they are active. Use the text chat for the references and report; use only an actually supported voice continuation path. For iOS, the documented paired-desktop path may be an option when enabled. Android voice integration remains to be checked on the user's actual app/account. Do not present keyboard dictation as equivalent to live voice or as sufficient audio evidence for pronunciation.

## Speaking interaction

Keep spoken instructions concise; do not read Markdown, score tables, filenames, code, history data, URLs or the entire corpus aloud. Read the entire Part 2 cue card once, then allow silent preparation. During the long turn, do not insert encouragement every few seconds. Stop your own speech if the candidate interrupts. Do not automatically end the phone call when the exam ends; the user may want feedback.

If voice activity detection segments a long answer, preserve the turn and wait for continuation. A model without accessible audio can still run the question sequence, but must withhold pronunciation and full FC scores. A UI showing a waveform is not proof that the assessing model receives the sound.

## Actual-device acceptance checklist

This checklist is pending until performed on each platform. It is not a claim of completed testing.

| Check | iOS | Android |
|---|---|---|
| Plugin selectable in a new chat | Pending | Pending |
| Uploaded Part 2 card retained in voice | Pending | Pending |
| One question per turn with uninterrupted long turn | Pending | Pending |
| Pause/resume preserves exam phase | Pending | Pending |
| All three parts completed | Pending | Pending |
| Audio evidence available to scoring model | Pending | Pending |
| Corpus-backed report and history accessible after voice | Pending | Pending |
| Blue/white icon assets respected by host | Pending | Pending |

A platform limitation is not solved by claiming support in the prompt. Report the affected step and retain all usable exam/reference functionality.
