---
api_specs:
- filename: acma-spectrum-licensing-openapi.yml
  format: yaml
  label: ACMA Spectrum Licensing API
  slug: spectrum-licensing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acma/refs/heads/main/openapi/acma-spectrum-licensing-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acma.gov.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: donotcall.gov.au
  spf: true
hosts:
- cert_expires: Sep 20 22:14:01 2026 GMT
  host: www.acma.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: developer.acma.gov.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: www.donotcall.gov.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ACMA, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ACMA
provider_slug: acma
slug: acma-domain-security
source_filename: acma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acma.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 22:14:01 2026 GMT\n  hsts: null\n- host: developer.acma.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.donotcall.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acma.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: donotcall.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acma/refs/heads/main/security/acma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Australia
- Regulator
- Spectrum
- Broadcasting
- Numbering
- Do Not Call Register
- Radiocommunications
- Licensing
- Open Data
- Government
- SOAP
---
