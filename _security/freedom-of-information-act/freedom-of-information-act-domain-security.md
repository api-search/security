---
api_specs:
- filename: freedom-of-information-act-openapi.yml
  format: yaml
  label: Freedom of Information Act (FOIA) API
  slug: freedom-of-information-act-foia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freedom-of-information-act/refs/heads/main/openapi/freedom-of-information-act-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: foia.gov
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: www.foia.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 13:20:52 2026 GMT
  host: api.foia.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freedom Of Information Act Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freedom of Information Act, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Freedom of Information Act
provider_slug: freedom-of-information-act
slug: freedom-of-information-act-domain-security
source_filename: freedom-of-information-act-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.foia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 13:20:52 2026 GMT\n  hsts: null\ndomains:\n- domain: foia.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freedom-of-information-act/refs/heads/main/security/freedom-of-information-act-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Federal Government
- FOIA
- Transparency
---
