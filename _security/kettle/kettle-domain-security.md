---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ourkettle.com
  spf: true
hosts:
- cert_expires: Sep 22 10:43:00 2026 GMT
  host: ourkettle.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kettle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kettle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kettle
provider_slug: kettle
slug: kettle-domain-security
source_filename: kettle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ourkettle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:43:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ourkettle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kettle/refs/heads/main/security/kettle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Reinsurance
- Climate
- Climate Risk
- Risk Modeling
- Machine Learning
---
