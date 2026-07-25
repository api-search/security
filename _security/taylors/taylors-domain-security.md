---
api_specs:
- filename: taylors-checkouts-api-openapi.yml
  format: yaml
  label: Taylor's University checkouts API
  slug: taylors-checkouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-checkouts-api-openapi.yml
- filename: taylors-holds-api-openapi.yml
  format: yaml
  label: Taylor's University holds API
  slug: taylors-holds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-holds-api-openapi.yml
- filename: taylors-item-types-api-openapi.yml
  format: yaml
  label: Taylor's University item_types API
  slug: taylors-item-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-item-types-api-openapi.yml
- filename: taylors-items-api-openapi.yml
  format: yaml
  label: Taylor's University items API
  slug: taylors-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-items-api-openapi.yml
- filename: taylors-libraries-api-openapi.yml
  format: yaml
  label: Taylor's University libraries API
  slug: taylors-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-libraries-api-openapi.yml
- filename: taylors-patrons-api-openapi.yml
  format: yaml
  label: Taylor's University patrons API
  slug: taylors-patrons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-patrons-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: taylors.edu.my
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: university.taylors.edu.my
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: librarycatalogue.taylors.edu.my
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: irepo.taylors.edu.my
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Taylors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taylor''s University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Taylor's University
provider_slug: taylors
slug: taylors-domain-security
source_filename: taylors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: university.taylors.edu.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: librarycatalogue.taylors.edu.my\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: false\n- host: irepo.taylors.edu.my\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: taylors.edu.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/security/taylors-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Library
- Institutional Repository
- Open Data
- Malaysia
- Asia
---
