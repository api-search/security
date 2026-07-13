---
api_specs:
- filename: finra-openapi.yml
  format: yaml
  label: FINRA Query API
  slug: query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finra/refs/heads/main/openapi/finra-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: finra.org
  spf: true
hosts:
- cert_expires: Sep 15 03:08:20 2026 GMT
  host: www.finra.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 03:29:21 2026 GMT
  host: developer.finra.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 09:41:59 2026 GMT
  host: api.finra.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FINRA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FINRA
provider_slug: finra
slug: finra-domain-security
source_filename: finra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.finra.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:08:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.finra.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:29:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.finra.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 09:41:59 2026 GMT\n  hsts: null\ndomains:\n- domain: finra.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finra/refs/heads/main/security/finra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- Financial
- Regulations
- Securities
- Market Data
---
