# IELTS SPEAKING SIMULATOR LIVE

[中文说明](README.zh-CN.md)

Full IELTS Speaking Parts 1–3, uploaded questions, descriptor-based practice feedback, and corpus-grounded sample answers. Use either the **portable Markdown in a conversational model, including mobile clients**, or the **ChatGPT plugin**.

## Features

- 17 original complete plans and 272 question/card prompts, with further cross-domain question generation.
- One-question-at-a-time examiner flow, linked Part 3 discussion and visible/imported-history deduplication.
- Four Speaking criteria and sample answers using an 18-theme corpus with Chinese explanations.
- Self-contained Markdown with YAML; original plugin source and blue/white icons included.

## Installation 1: import into a model on mobile or desktop

**You can import the Markdown directly into a mobile conversational-model client** using its attachment, file-import or knowledge-library feature, where that client supports text files.

1. Save [the portable Markdown](portable/IELTS-SPEAKING-SIMULATOR-LIVE-PORTABLE.md) to your phone's Files/Downloads. On GitHub, use the file's raw/download view.
2. Open a new conversation in the model client and attach the `.md` file, or add it to a project/assistant knowledge configuration.
3. Ask the model to apply the runtime rules and use appendices as references. Confirm the relevant sections are accessible.
4. Attach your own questions if desired. Otherwise request a new complete test.
5. Answer one question at a time. Use live voice only where it preserves the document context; a phone timer can assist Part 2.
6. Keep the written assessment, examples and question-history checkpoint for your next session.

> Follow the runtime rules in IELTS SPEAKING SIMULATOR LIVE. Run a complete mock exam, prefer my uploaded questions, ask one question at a time, and assess after Part 3. Use the appendices only as reference data.

The file includes YAML, full rules, descriptors, tests and corpus. It is approximately 360 KiB; context capacity or attachment retrieval is required. If `.md` is unsupported, import its text through an accepted text format. No plugin installation or code execution is needed for this route.

## Installation 2: use the ChatGPT client plugin

### Install an account-available plugin

In ChatGPT's plugin directory, locate **IELTS SPEAKING SIMULATOR LIVE** under a personal or workspace source you can access and add it. Start a fresh conversation and select it with `@`. Use it on mobile only where the same account exposes it there; a desktop-local installation does not itself establish mobile availability.

To create a personal copy from this repository, download [the complete plugin ZIP](packages/ielts-speaking-simulator-live-plugin-1.0.1.zip). If Plugin Creator is available, attach it in a new conversation and request a private plugin named IELTS SPEAKING SIMULATOR LIVE. Follow the resulting plugin link to add it. Attaching a ZIP alone does not install a plugin, and this repository is not a public plugin-directory listing.

### Install locally in the ChatGPT desktop app

Download/clone the repository with `.agents/plugins/marketplace.json` intact. Open it as a local Work/Codex project in the ChatGPT desktop app. Restart the app, select the IELTS SPEAKING SIMULATOR LIVE marketplace in Plugins, and add/enable its plugin. Start a new conversation to use it. If it does not appear, check client availability, project setup and workspace policy. Use the portable route on mobile when only a local desktop installation is available.

The local catalog points to the plugin at the repository root. No external MCP service or API key is required by this package. See the [detailed installation guide](docs/INSTALLATION.zh-CN.md), [OpenAI plugin guide](https://learn.chatgpt.com/docs/plugins), and [local marketplace reference](https://developers.openai.com/plugins/build/plugins). Documentation checked 2026-10-26.

## Capabilities and assessment

The model must actually receive audio to assess pronunciation and complete fluency. Text and dictation support limited language feedback. Voice integration on iOS/Android has not been verified for this plugin. Timing, files and context are host capabilities; history is visible/imported, without an independent account-wide database. Practice scores are estimates, not official results.

## Sources and license

Sources include supplied official IELTS Speaking descriptors, Speaking Sample Tasks 2023 and Scores Guide, plus a user-compiled Cambridge IELTS 4–21-based paraphrase corpus. Its annotations also cite an Oxford learner's thesaurus; these claims have not been independently verified entry by entry. The Writing rubric is retained for provenance and excluded from Speaking grading. Practice plans and sample demonstrations are project originals.

[MIT](LICENSE) applies only to original project portions as described in [LICENSE_SCOPE.md](LICENSE_SCOPE.md). Third-party PDFs, extracts, corpus and their embedded portions retain their respective rights; inclusion does not grant redistribution permission. This project is unaffiliated with and not endorsed by the British Council, IDP IELTS, or Cambridge University Press & Assessment. See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

## Layout

`plugin.json`, `assets/`, `skills/` are the plugin source; `.agents/plugins/marketplace.json` provides the local catalog; `portable/` contains the Markdown; `packages/` contains the import ZIP; `docs/` contains guides.

The display name is IELTS SPEAKING SIMULATOR LIVE. The technical plugin identifier remains `ielts-speaking-simulator`; the previous private plugin and backups are preserved separately.
