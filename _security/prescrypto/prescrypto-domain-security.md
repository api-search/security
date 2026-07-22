---
api_specs:
- filename: prescrypto-openapi.yml
  format: yaml
  label: Prescrypto Integration API
  slug: prescrypto-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prescrypto/refs/heads/main/openapi/prescrypto-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prescrypto.com
  spf: true
hosts:
- cert_expires: Sep 10 06:51:31 2026 GMT
  host: prescrypto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prescrypto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prescrypto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prescrypto
provider_slug: prescrypto
slug: prescrypto-domain-security
source_filename: prescrypto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prescrypto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:51:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: prescrypto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prescrypto/refs/heads/main/security/prescrypto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Electronic Prescriptions
- eRx
- Pharmacy
- Telemedicine
- Medical
- Mexico
- LATAM
---
