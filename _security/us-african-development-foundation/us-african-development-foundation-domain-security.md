---
api_specs:
- filename: usadf-grants-api-openapi.yml
  format: yaml
  label: USADF Grants Data API
  slug: grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-african-development-foundation/refs/heads/main/openapi/usadf-grants-api-openapi.yml
- filename: usadf-grant-opportunities-api-openapi.yml
  format: yaml
  label: USADF Grant Opportunities API
  slug: grant-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-african-development-foundation/refs/heads/main/openapi/usadf-grant-opportunities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usadf.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usaspending.gov
  spf: true
hosts:
- cert_expires: Aug  2 23:43:41 2026 GMT
  host: www.usadf.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: www.usaspending.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api.usaspending.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Us African Development Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US African Development Foundation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US African Development Foundation
provider_slug: us-african-development-foundation
slug: us-african-development-foundation-domain-security
source_filename: us-african-development-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usadf.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 23:43:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.usaspending.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usaspending.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usadf.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: usaspending.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-african-development-foundation/refs/heads/main/security/us-african-development-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- International Development
- Africa
- Grants
- Nonprofit
- Economic Development
---
