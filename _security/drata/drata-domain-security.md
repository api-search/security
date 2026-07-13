---
api_specs:
- filename: drata-openapi.yml
  format: yaml
  label: Drata Public API v2
  slug: public-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: drata.com
  spf: true
hosts:
- cert_expires: Oct  7 03:49:09 2026 GMT
  host: drata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:49:09 2026 GMT
  host: developers.drata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:49:09 2026 GMT
  host: public-api.drata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drata, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Drata
provider_slug: drata
slug: drata-domain-security
source_filename: drata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:49:09 2026 GMT\n  hsts: null\n- host: developers.drata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:49:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api.drata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:49:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: drata.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/security/drata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- GRC
- Compliance
- SOC 2
- ISO 27001
- Security
---
