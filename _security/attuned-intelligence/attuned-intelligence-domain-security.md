---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: attuned-intelligence.com
  spf: true
hosts:
- cert_expires: Sep  2 16:22:49 2026 GMT
  host: www.attuned-intelligence.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Attuned Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Attuned Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Attuned Intelligence
provider_slug: attuned-intelligence
slug: attuned-intelligence-domain-security
source_filename: attuned-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.attuned-intelligence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 16:22:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: attuned-intelligence.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attuned-intelligence/refs/heads/main/security/attuned-intelligence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Healthcare
- Voice AI
- Call Center Automation
- EHR Integration
- Conversational AI
- HIPAA
---
