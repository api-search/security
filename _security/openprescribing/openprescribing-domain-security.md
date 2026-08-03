---
api_specs:
- filename: openprescribing-openapi.yml
  format: yaml
  label: OpenPrescribing API
  slug: openprescribing-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openprescribing/refs/heads/main/openapi/openprescribing-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openprescribing.net
  spf: true
hosts:
- cert_expires: Oct  5 12:18:45 2026 GMT
  host: openprescribing.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openprescribing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenPrescribing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenPrescribing
provider_slug: openprescribing
slug: openprescribing-domain-security
source_filename: openprescribing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openprescribing.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:18:45 2026 GMT\n  hsts: false\ndomains:\n- domain: openprescribing.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openprescribing/refs/heads/main/security/openprescribing-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- United Kingdom
- NHS
- Prescribing
- Pharmacy
- Open Data
- Primary Care
- Public Health
- Analytics
---
