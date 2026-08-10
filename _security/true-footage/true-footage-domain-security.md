---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: truefootage.tech
  spf: true
hosts:
- cert_expires: Oct 30 07:56:59 2026 GMT
  host: www.truefootage.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 04:22:03 2026 GMT
  host: api.truetracts.truefootage.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 14:00:24 2026 GMT
  host: api.trueengine.truefootage.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: True Footage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for True Footage, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: True Footage
provider_slug: true-footage
slug: true-footage-domain-security
source_filename: true-footage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.truefootage.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 07:56:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.truetracts.truefootage.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 04:22:03 2026 GMT\n  hsts: null\n- host: api.trueengine.truefootage.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 14:00:24 2026 GMT\n  hsts: null\ndomains:\n- domain: truefootage.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/true-footage/refs/heads/main/security/true-footage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Appraisal
- Valuation
- PropTech
- Mortgage
- Property Data
- Analytics
- Machine Learning
---
