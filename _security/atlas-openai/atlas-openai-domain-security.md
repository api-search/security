---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openai.com
  spf: true
hosts:
- cert_expires: Aug 26 19:33:25 2026 GMT
  host: openai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atlas Openai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChatGPT Atlas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ChatGPT Atlas
provider_slug: atlas-openai
slug: atlas-openai-domain-security
source_filename: atlas-openai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 19:33:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openai.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlas-openai/refs/heads/main/security/atlas-openai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Browser
- Consumer
- Agent
- Chromium
- ChatGPT
- OpenAI
---
