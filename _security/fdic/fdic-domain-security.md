---
api_specs:
- filename: swagger.yaml
  format: yaml
  label: FDIC BankFind Suite API
  slug: bankfind
  spec_type: OpenAPI
  url: https://api.fdic.gov/banks/docs/swagger.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fdic.gov
  spf: true
hosts:
- cert_expires: Aug 17 15:32:11 2026 GMT
  host: www.fdic.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 21:21:32 2026 GMT
  host: banks.data.fdic.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 13:21:07 2026 GMT
  host: api.fdic.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fdic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FDIC, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FDIC
provider_slug: fdic
slug: fdic-domain-security
source_filename: fdic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fdic.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:32:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: banks.data.fdic.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 21:21:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fdic.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 13:21:07 2026 GMT\n  hsts: null\ndomains:\n- domain: fdic.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fdic/refs/heads/main/security/fdic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Finance
- Government
- FDIC
- Financial Data
- Bank Data
- Regulatory
---
