# DocuPrune for Codex

Convert chosen documents through [DocuPrune](https://docuprune.com), review their
actual results, and save Markdown or batch ZIP files from a compatible desktop
browser session.

This is the direct DocuPrune plugin distribution. It is **not a listing or
approval in OpenAI's public plugin directory**.

## Install

Use a Codex build that supports plugin marketplace commands. In your terminal:

```sh
codex plugin marketplace add https://github.com/AbanoubIbrahimYounan/docuprune-codex-plugin.git
codex plugin add docuprune@docuprune
```

Open a new local desktop conversation and select DocuPrune from the plugin menu,
or invoke its skill:

```text
Use $docuprune to convert my chosen document through the website and save Markdown.
```

For a first test without a private document:

```text
Use $docuprune to try a public sample, inspect the actual result and save the export.
```

Browser control and access to your chosen files must be available in the session.
If a native Save dialog needs your confirmation, complete that step; a click
without a saved file does not establish success. Browser extensions and download
integrations can interfere with sample loading or saving. Keep normal browser
security and permission settings in place and report the specific failed step.

## What is included

- One browser workflow skill, with instructions for file selection, sample use,
  completed-row checks, review, single-file downloads and batch archive checks.
- The current DocuPrune leaf icons.
- A marketplace catalog for installing the workflow in Codex.

The website and conversion engine are **not included in this repository**. There
is no bundled converter, public converter CLI, MCP server, upload service, hook,
API key or install script. The private website repository and its history are
not part of this distribution.

## Check the result

Keep your original document. Review important headings, table columns, numbers
and edited passages against it. OCR, complex layouts and Arabic-Indic numerals
can need manual review. A completed row or successful download does not prove
that every extracted character is correct. Partial or failed files should be
reported explicitly, rather than called a completed batch.

## Privacy and support

Conversion happens in the website's browser workspace. Content an assistant
reads or returns to the conversation is available to the assistant and its
platform; browser processing does not keep that returned content exclusively
inside the website. Ask for download-only output when appropriate.

- [About the plugin](https://docuprune.com/plugins/docuprune)
- [Privacy notice](https://docuprune.com/plugins/docuprune/privacy)
- [Support](https://docuprune.com/plugins/docuprune/support)
- Contact: [abanoubibrahim35@gmail.com](mailto:abanoubibrahim35@gmail.com)

Use synthetic or public samples when reporting problems. Do not send passwords,
access tokens, identity documents or confidential files to support.

## Updates

```sh
codex plugin marketplace upgrade docuprune
codex plugin add docuprune@docuprune
```

The website's engine is updated separately from this instruction package.

## Use and ownership

You may download and install this plugin to use DocuPrune. The website and
conversion engine remain separate proprietary software; no right to their
source code is granted by this distribution. Brand assets identify DocuPrune.

Marketplace format and command references:
[Plugin packaging](https://developers.openai.com/plugins/build/plugins#marketplace-metadata)
and [developer commands](https://learn.chatgpt.com/docs/developer-commands#codex-plugin-marketplace).
