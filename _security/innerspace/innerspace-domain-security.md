---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: innerspace.io
  spf: true
hosts:
- cert_expires: Oct 11 05:25:09 2026 GMT
  host: innerspace.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 01:34:08 2026 GMT
  host: developers.innerspace.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 01:28:35 2026 GMT
  host: api.innerspace.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Innerspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InnerSpace, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: InnerSpace
provider_slug: innerspace
slug: innerspace-domain-security
source_filename: innerspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: innerspace.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 05:25:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.innerspace.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 01:34:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.innerspace.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 01:28:35 2026 GMT\n  hsts: null\ndomains:\n- domain: innerspace.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innerspace/refs/heads/main/security/innerspace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Workplace Analytics
- Occupancy
- Space Utilization
- Real Estate
- Wi-Fi Location
- Building Insights
- GraphQL
- Hybrid Workplace
- PropTech
---
