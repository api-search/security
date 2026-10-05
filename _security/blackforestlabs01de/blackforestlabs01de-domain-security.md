---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: equityzen.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bfl.ai
  spf: false
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: equityzen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 05:40:07 2026 GMT
  host: bfl.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: api.bfl.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Blackforestlabs01De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blackforestlabs01de, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blackforestlabs01de
provider_slug: blackforestlabs01de
slug: blackforestlabs01de-domain-security
source_filename: blackforestlabs01de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: equityzen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\n- host: bfl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 05:40:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.bfl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: equityzen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: bfl.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackforestlabs01de/refs/heads/main/security/blackforestlabs01de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Technology
- Data
- Artificial Intelligence
- Research
---
