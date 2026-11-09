---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buyhongkonginsurance.com
  spf: true
hosts:
- cert_expires: Jan  9 16:10:15 2027 GMT
  host: buyhongkonginsurance.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buyhongkonginsurance Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hong Kong Insurance Connect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hong Kong Insurance Connect
provider_slug: buyhongkonginsurance-com
slug: buyhongkonginsurance-com-domain-security
source_filename: buyhongkonginsurance-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buyhongkonginsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 16:10:15 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: buyhongkonginsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/buyhongkonginsurance-com/security/buyhongkonginsurance-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Hong Kong
- Comparison
- Brokerage
- Finance
---
