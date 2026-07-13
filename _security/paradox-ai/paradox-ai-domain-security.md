---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:paradox-devops@workday.com"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "microsoft.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paradox.ai
  spf: true
hosts:
- cert_expires: Aug 16 14:56:36 2026 GMT
  host: www.paradox.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: app.paradox.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Paradox Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paradox, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paradox
provider_slug: paradox-ai
slug: paradox-ai-domain-security
source_filename: paradox-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paradox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 14:56:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.paradox.ai\n  https: false\ndomains:\n- domain: paradox.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:paradox-devops@workday.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paradox-ai/refs/heads/main/security/paradox-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Conversational AI
- Recruiting Automation
- High-Volume Hiring
- Chatbot
- ATS
- HR Tech
---
