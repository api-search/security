---
certifications:
- read
- published
- note
description: ''
kind: trust-center
layout: security
name: Zefr Trust Center
name_suffix: Trust Center
overview: Zefr maintains a public trust center documenting read, published, and note compliance.
provider_name: Zefr
provider_slug: zefr
slug: zefr-trust-center
source_filename: zefr-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://trust.zefr.com/\npresent: true\nplatform: Drata\nurl: https://trust.zefr.com/\nnote: >-\n  Zefr operates a trust center. It is provisioned on a Zefr-controlled hostname\n  (trust.zefr.com) that CNAMEs to trust.cname.drata.com — Drata's hosted Trust Center\n  product — and the page is publicly indexed under the title \"Trust Center | Powered by\n  Drata\". The document itself could NOT be read: trust.zefr.com sits behind a Cloudflare\n  bot challenge that answers HTTP 403 with a \"Just a moment...\" interstitial to every\n  non-browser client, including a browser-UA curl and the fetch tool. We do not evade\n  challenges. Presence is therefore asserted; contents are not.\nevidence:\n- kind: dns\n  record: CNAME\n  name: trust.zefr.com\n  value: trust.cname.drata.com\n  note: Drata Trust Center hosted endpoint on a Zefr-controlled hostname.\n- kind: http\n  url: https://trust.zefr.com/\n  status: 403\n  content_type: text/html;\
  \ charset=UTF-8\n  body_signature: Cloudflare managed challenge (\"Just a moment...\", challenges.cloudflare.com CSP)\n- kind: http\n  url: https://trust.zefr.com/api/trust-center/zefr\n  status: 403\n- kind: search-index\n  query: site:trust.zefr.com\n  result: 'Indexed page title: \"Trust Center | Powered by Drata\"'\ncertifications:\n  read: false\n  published: []\n  note: >-\n    NO certification is asserted. SOC 2, ISO 27001, PCI DSS, HIPAA and similar are commonly\n    surfaced by Drata trust centers, but none was read from Zefr's, so none is recorded.\n    A reader who needs Zefr's certification list must open trust.zefr.com in a browser.\nsubprocessors:\n  read: false\ndocuments_on_request:\n  read: false\ncoverage:\n  state: blocked\n  reason: bot-challenge\n  detail: >-\n    trust.zefr.com returns a Cloudflare managed challenge (HTTP 403) to every non-browser\n    client, so the trust center's certification list could not be read.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zefr/refs/heads/main/security/zefr-trust-center.yml
summary_line: read, published, note
tags:
- Company
- Adtech
- Brand Safety
- Brand Suitability
- Content Intelligence
- Content Moderation
- Video
- Social Media
- Advertising
- Media Measurement
- Machine Learning
trust_url: https://trust.zefr.com/
---
