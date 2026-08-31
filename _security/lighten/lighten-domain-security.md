---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lighten-ai.com
  spf: false
hosts:
- cert_expires: Sep 30 20:23:00 2026 GMT
  host: lighten-ai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lighten Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lighten, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Lighten
provider_slug: lighten
slug: lighten-domain-security
source_filename: lighten-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lighten-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:23:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lighten-ai.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lighten/refs/heads/main/security/lighten-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Life Sciences
- Artificial Intelligence
- Electronic Health Records
- Real World Evidence
- Clinical Data
- Data Curation
---
