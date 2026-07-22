---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tsenta.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: autojobs.me
  spf: false
hosts:
- cert_expires: Sep 15 23:35:49 2026 GMT
  host: tsenta.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 11:10:01 2026 GMT
  host: docs.tsenta.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 11:13:18 2026 GMT
  host: api.autojobs.me
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tsenta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tsenta, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tsenta
provider_slug: tsenta
slug: tsenta-domain-security
source_filename: tsenta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tsenta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:35:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.tsenta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 11:10:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.autojobs.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 11:13:18 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: tsenta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: autojobs.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tsenta/refs/heads/main/security/tsenta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Jobs
- Recruiting
- Job Search
- AI Agents
- Automation
- Applicant Tracking
- Career
- MCP
- Y Combinator
---
