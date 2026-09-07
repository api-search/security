---
description: ''
domains:
- caa:
  - 0 iodef "mailto:wand-it-devops@wand.ai"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wand.ai
  spf: true
hosts:
- cert_expires: Oct 31 02:51:16 2026 GMT
  host: wand.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 12:31:50 2026 GMT
  host: status.wand.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 09:09:51 2026 GMT
  host: auth.wand.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Wand Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wand, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wand
provider_slug: wand-ai
slug: wand-ai-domain-security
source_filename: wand-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wand.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 02:51:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: status.wand.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 12:31:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: auth.wand.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 09:09:51 2026 GMT\n  hsts: null\ndomains:\n- domain: wand.ai\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:wand-it-devops@wand.ai\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wand-ai/refs/heads/main/security/wand-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agentic AI
- Enterprise Software
- Workforce Automation
- Orchestration
- Process Automation
- Collaboration
- Governance
---
