---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:security@unframe.ai"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unframe.ai
  spf: true
hosts:
- cert_expires: Sep  9 17:17:12 2026 GMT
  host: www.unframe.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unframe Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unframe AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unframe AI
provider_slug: unframe-ai
slug: unframe-ai-domain-security
source_filename: unframe-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unframe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 17:17:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unframe.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:security@unframe.ai\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unframe-ai/refs/heads/main/security/unframe-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Enterprise AI
- Agentic AI
- AI Agents
- Workflow Automation
- Voice Agents
---
