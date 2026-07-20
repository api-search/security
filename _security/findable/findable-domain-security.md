---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: findable.ai
  spf: true
hosts:
- cert_expires: Sep 11 04:05:11 2026 GMT
  host: www.findable.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 20:56:56 2026 GMT
  host: docs.findable.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 05:21:26 2026 GMT
  host: api.findable.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Findable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Findable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Findable
provider_slug: findable
slug: findable-domain-security
source_filename: findable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.findable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:05:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.findable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 20:56:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.findable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:21:26 2026 GMT\n  hsts: null\ndomains:\n- domain: findable.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/findable/refs/heads/main/security/findable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Building Intelligence
- Property Technology
- PropTech
- Facilities Management
- Building Documentation
- Compliance
- Artificial Intelligence
- Document Search
- Construction
---
