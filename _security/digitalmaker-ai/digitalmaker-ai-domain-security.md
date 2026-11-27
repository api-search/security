---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: digitalmaker.ai
  spf: true
hosts:
- cert_expires: Dec 27 02:39:51 2026 GMT
  host: digitalmaker.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Digital Maker AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digital Maker AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Digital Maker AI
provider_slug: digitalmaker-ai
slug: digitalmaker-ai-domain-security
source_filename: digitalmaker-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digitalmaker.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 02:39:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: digitalmaker.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/digitalmaker-ai/security/digitalmaker-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Video Generation
- Faceless Video
- YouTube
- Content Creation
- Digital Products
- MCP
---
