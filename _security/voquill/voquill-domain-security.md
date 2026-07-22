---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: voquill.com
  spf: true
hosts:
- cert_expires: Aug 30 05:24:44 2026 GMT
  host: voquill.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voquill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voquill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Voquill
provider_slug: voquill
slug: voquill-domain-security
source_filename: voquill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voquill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 05:24:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: voquill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voquill/refs/heads/main/security/voquill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Voice
- Dictation
- Speech-to-Text
- AI
- Open Source
- Healthcare
- Pathology
- Productivity
---
