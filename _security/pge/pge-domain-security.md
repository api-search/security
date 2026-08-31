---
api_specs:
- filename: pge-applicationinformation-api-openapi.yml
  format: yaml
  label: Pacific Gas and Electric Application Information API
  slug: pge-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/openapi/pge-applicationinformation-api-openapi.yml
- filename: pge-authorization-api-openapi.yml
  format: yaml
  label: Pacific Gas and Electric Authorization API
  slug: pge-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/openapi/pge-authorization-api-openapi.yml
- filename: pge-batch-api-openapi.yml
  format: yaml
  label: Pacific Gas and Electric Batch API
  slug: pge-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/openapi/pge-batch-api-openapi.yml
- filename: pge-usagepoint-api-openapi.yml
  format: yaml
  label: Pacific Gas and Electric Usage Point API
  slug: pge-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/openapi/pge-usagepoint-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pge.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greenbuttonalliance.org
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.pge.com
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 12 23:59:59 2027 GMT
  host: api.pge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 20:26:53 2026 GMT
  host: sandbox.greenbuttonalliance.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pacific Gas and Electric, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pacific Gas and Electric
provider_slug: pge
slug: pge-domain-security
source_filename: pge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2628000\n- host: api.pge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 12 23:59:59 2027 GMT\n  hsts: null\n- host: sandbox.greenbuttonalliance.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:26:53 2026 GMT\n  hsts: null\ndomains:\n- domain: pge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: greenbuttonalliance.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/security/pge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Utilities
- Electricity
- Gas
- California
- Smart Metering
- Green Button
- ESPI
- Energy Data
- Grid
- Demand Response
- Investor-Owned Utility
---
