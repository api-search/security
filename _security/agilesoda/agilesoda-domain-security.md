---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agilesoda.ai
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: agilesoda.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: docs.agilesoda.ai
  https: false
  note: Port 443 is closed/filtered; the documentation portal is served only over plaintext HTTP (http://docs.agilesoda.ai/agiledocs_ko) and its per-guide login form posts credentials to /r/signon/login over that same unencrypted channel. Probed 2026-09-12.
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Agilesoda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgileSoDA, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AgileSoDA
provider_slug: agilesoda
slug: agilesoda-domain-security
source_filename: agilesoda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agilesoda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\n- host: docs.agilesoda.ai\n  https: false\n  note: >-\n    Port 443 is closed/filtered; the documentation portal is served only over plaintext HTTP\n    (http://docs.agilesoda.ai/agiledocs_ko) and its per-guide login form posts credentials to\n    /r/signon/login over that same unencrypted channel. Probed 2026-09-12.\ndomains:\n- domain: agilesoda.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agilesoda/refs/heads/main/security/agilesoda-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- AI Agents
- Machine-Learning
- Enterprise Software
- Document Processing
- Optical Character Recognition
- RAG
- Reinforcement Learning
- Insurance
- South Korea
---
