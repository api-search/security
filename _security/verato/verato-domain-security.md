---
api_specs:
- filename: verato-person-openapi.yml
  format: yaml
  label: Verato Person API
  slug: verato-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verato/refs/heads/main/openapi/verato-person-openapi.yml
- filename: verato-organization-openapi.yml
  format: yaml
  label: Verato Organization API
  slug: verato-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verato/refs/heads/main/openapi/verato-organization-openapi.yml
- filename: verato-provider-openapi.yml
  format: yaml
  label: Verato Provider API
  slug: verato-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verato/refs/heads/main/openapi/verato-provider-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verato.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: yourveratodomain.com
  spf: false
hosts:
- cert_expires: Sep 14 16:31:34 2026 GMT
  host: verato.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 15:36:08 2026 GMT
  host: developer.verato.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: yourveratodomain.com
  https: false
kind: domain-security
layout: security
method: probed
name: Verato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verato, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verato
provider_slug: verato
slug: verato-domain-security
source_filename: verato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 16:31:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.verato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 15:36:08 2026 GMT\n  hsts: false\n- host: yourveratodomain.com\n  https: false\ndomains:\n- domain: verato.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: yourveratodomain.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verato/refs/heads/main/security/verato-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Healthcare
- Identity
- Identity Resolution
- Master Data Management
- Patient Matching
- Provider Data Management
- Data Quality
- EMPI
---
