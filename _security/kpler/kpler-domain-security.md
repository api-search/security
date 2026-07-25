---
api_specs:
- filename: kpler-aggregations-api-openapi.yml
  format: yaml
  label: Kpler Aggregations API
  slug: kpler-aggregations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/openapi/kpler-aggregations-api-openapi.yml
- filename: kpler-authentication-api-openapi.yml
  format: yaml
  label: Kpler Authentication API
  slug: kpler-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/openapi/kpler-authentication-api-openapi.yml
- filename: kpler-facts-api-openapi.yml
  format: yaml
  label: Kpler Facts API
  slug: kpler-facts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/openapi/kpler-facts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kpler.com
  spf: true
hosts:
- cert_expires: Aug 22 02:44:31 2026 GMT
  host: www.kpler.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 08:43:43 2026 GMT
  host: liquids.dev.kpler.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: api.kpler.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kpler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kpler, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kpler
provider_slug: kpler
slug: kpler-domain-security
source_filename: kpler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kpler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:44:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: liquids.dev.kpler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 08:43:43 2026 GMT\n  hsts: null\n- host: api.kpler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kpler.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/security/kpler-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Vessel Tracking
- Maritime
- Commodities
- Supply Chain
- AIS
- Trade Flows
- Shipping
- Energy
---
