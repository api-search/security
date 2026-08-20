---
api_specs:
- filename: fixflo-api-v2-openapi.yml
  format: yaml
  label: Fixflo API v2
  slug: fixflo-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixflo/refs/heads/main/openapi/fixflo-api-v2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fixflo.com
  spf: true
hosts:
- cert_expires: Sep 19 12:08:47 2026 GMT
  host: www.fixflo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: api-docs.fixflo.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 10:38:08 2026 GMT
  host: api-sandbox.fixflo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fixflo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fixflo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fixflo
provider_slug: fixflo
slug: fixflo-domain-security
source_filename: fixflo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fixflo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 12:08:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.fixflo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: api-sandbox.fixflo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 10:38:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fixflo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fixflo/refs/heads/main/security/fixflo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United Kingdom
- Property Management
- PropTech
- Repairs and Maintenance
- Block Management
- Lettings
- Rentals
- Commercial Real Estate
- Contractors
---
