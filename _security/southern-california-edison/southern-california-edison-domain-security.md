---
api_specs:
- filename: southern-california-edison-drpep-portal-api-openapi.yml
  format: yaml
  label: Southern California Edison DRPEP Portal API
  slug: southern-california-edison-drpep-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/southern-california-edison/refs/heads/main/openapi/southern-california-edison-drpep-portal-api-openapi.yml
- filename: southern-california-edison-feature-services-api-openapi.yml
  format: yaml
  label: Southern California Edison Feature Services API
  slug: southern-california-edison-feature-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/southern-california-edison/refs/heads/main/openapi/southern-california-edison-feature-services-api-openapi.yml
- filename: southern-california-edison-query-api-openapi.yml
  format: yaml
  label: Southern California Edison Query API
  slug: southern-california-edison-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/southern-california-edison/refs/heads/main/openapi/southern-california-edison-query-api-openapi.yml
- filename: southern-california-edison-server-api-openapi.yml
  format: yaml
  label: Southern California Edison Server API
  slug: southern-california-edison-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/southern-california-edison/refs/heads/main/openapi/southern-california-edison-server-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sce.com
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: www.sce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: drpep.sce.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Southern California Edison Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Southern California Edison, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Southern California Edison
provider_slug: southern-california-edison
slug: southern-california-edison-domain-security
source_filename: southern-california-edison-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: drpep.sce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: sce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/southern-california-edison/refs/heads/main/security/southern-california-edison-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Utilities
- Electricity
- Smart Metering
- Green Button
- Grid
- Demand Response
- Solar
- DER
- EV Charging
- California
---
