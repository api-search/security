---
api_specs:
- filename: sentera-graphql-api-openapi.yml
  format: yaml
  label: Sentera GraphQL API
  slug: sentera-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentera/refs/heads/main/openapi/sentera-graphql-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sentera.com
  spf: true
hosts:
- cert_expires: Oct 30 20:51:32 2026 GMT
  host: sentera.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 30 20:51:32 2026 GMT
  host: api.sentera.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sentera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sentera, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sentera
provider_slug: sentera
slug: sentera-domain-security
source_filename: sentera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sentera.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 20:51:32 2026 GMT\n  hsts: false\n- host: api.sentera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 20:51:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sentera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentera/refs/heads/main/security/sentera-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Precision Agriculture
- Aerial Imagery
- Drones
- Sensors
- Analytics
- GraphQL
---
