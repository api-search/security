---
api_specs:
- filename: careranks-com-openapi-generated.yml
  format: yaml
  label: CareRanks API
  slug: careranks-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/careranks-com/openapi/_ae-authored/careranks-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: careranks.com
  spf: true
hosts:
- cert_expires: Dec 27 17:59:52 2026 GMT
  host: careranks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Careranks Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CareRanks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CareRanks
provider_slug: careranks-com
slug: careranks-com-domain-security
source_filename: careranks-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: careranks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 17:59:52 2026 GMT\n  hsts: false\ndomains:\n- domain: careranks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/careranks-com/security/careranks-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Transparency
- Data
- Hospitals
- Pricing
---
