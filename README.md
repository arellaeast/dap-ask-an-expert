# Ask a DAP Expert (Concept Demo)

A 24/7 product-help chat styled to fit the DAP brand. Every answer is grounded in DAP published material and cites its source. Nothing is improvised.

**Live demo:** https://arellaeast.github.io/dap-ask-an-expert/

Part of a three-piece demo suite by Jacob East:
- Product Finder: https://arellaeast.github.io/dap-product-finder/
- Ask a DAP Expert: https://arellaeast.github.io/dap-ask-an-expert/
- Sealant Calculator: https://arellaeast.github.io/dap-sealant-calculator/

## The point of this demo

Research for a Website Manager application at DAP Global found:

- DAP offers expert help only through human contact, while Gorilla runs a 24/7 AI assistant that gives instant product recommendations
- The same questions repeat across DAP's 1-star reviews and support replies: Can I use Alex Plus in a shower? Why did it crack? Why is my clear caulk still white? How do I claim the warranty?
- DAP already has the answers, in its FAQs, technical data sheets and review replies. They are just not available at 11 pm before a Saturday job

This chat answers those questions from that corpus, cites the source under every answer, and hands anything outside the base to a human at the number DAP itself publishes (888-327-8477). It includes one Spanish answer as a pilot, since dap.com has no US Spanish experience yet.

## How it works

`kb.js` holds the knowledge base as data plus a pure `matchAnswer(query)` function, so the matching can be unit tested. Entries are ordered most specific first. A production version would ground an AI assistant in the same FAQ/TDS corpus with the same rule: cite it or do not say it.

## Run it locally

No build step. Open `index.html` in a browser, or serve the folder with `python3 -m http.server`.

## Disclaimer

Independent concept prototype. Not an official DAP product, and not affiliated with or endorsed by DAP Products Inc. or RPM International. Always check the label and technical data sheet for your specific job.
