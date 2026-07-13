---
api_specs:
- filename: ecfr-openapi.json
  format: json
  label: eCFR Versioner API
  slug: versioner
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecfr/refs/heads/main/openapi/ecfr-openapi.json
- filename: ecfr-openapi.json
  format: json
  label: eCFR Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecfr/refs/heads/main/openapi/ecfr-openapi.json
- filename: ecfr-openapi.json
  format: json
  label: eCFR Admin API
  slug: admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecfr/refs/heads/main/openapi/ecfr-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ecfr.gov
  spf: true
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: www.ecfr.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ecfr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eCFR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: eCFR
provider_slug: ecfr
slug: ecfr-domain-security
source_filename: ecfr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ecfr.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ecfr.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecfr/refs/heads/main/security/ecfr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Regulations
- Government
- Legal
- Compliance
- Open Data
- United States
---
