---
api_specs:
- filename: toronto-hydro-applicationinformation-api-openapi.yml
  format: yaml
  label: Toronto Hydro Application Information API
  slug: toronto-hydro-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/openapi/toronto-hydro-applicationinformation-api-openapi.yml
- filename: toronto-hydro-authorization-api-openapi.yml
  format: yaml
  label: Toronto Hydro Authorization API
  slug: toronto-hydro-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/openapi/toronto-hydro-authorization-api-openapi.yml
- filename: toronto-hydro-batch-api-openapi.yml
  format: yaml
  label: Toronto Hydro Batch API
  slug: toronto-hydro-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/openapi/toronto-hydro-batch-api-openapi.yml
- filename: toronto-hydro-usagepoint-api-openapi.yml
  format: yaml
  label: Toronto Hydro Usage Point API
  slug: toronto-hydro-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/openapi/toronto-hydro-usagepoint-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: torontohydro.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greenbuttonalliance.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: savagedata.com
  note: Platform vendor domain hosting Toronto Hydro's Green Button third-party onboarding application.
  probed_manually: true
  spf: true
hosts:
- cert_expires: Sep 23 06:32:21 2026 GMT
  host: www.torontohydro.com
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 20:26:53 2026 GMT
  host: sandbox.greenbuttonalliance.org
  hsts: null
  https: true
  note: servers[] host of the harvested Green Button Alliance OpenAPI in this repo. Not a Toronto Hydro host.
  tls_version: TLSv1.3
- cert_expires: Nov 17 14:06:38 2026 GMT
  host: torontoonboarding.savagedata.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: Added by hand because the host is carried as DeveloperPortal/SignUp rather than Website, so the automated host collector did not reach it. This is the third-party Green Button onboarding application Toronto Hydro links to from its public Green Button page, operated by its platform vendor Savage Data Systems. It negotiates TLSv1.2 only (no TLSv1.3) and advertises a 30-day HSTS max-age — a weaker posture than Toronto Hydro's own www host, on the surface a developer must actually use.
  probed_manually: true
  server: Microsoft-IIS/10.0
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Toronto Hydro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toronto Hydro, probed live across 3 host(s) and 3 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Toronto Hydro
provider_slug: toronto-hydro
slug: toronto-hydro-domain-security
source_filename: toronto-hydro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.torontohydro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:32:21 2026 GMT\n  hsts: true\n  hsts_max_age: 157680000\n- host: sandbox.greenbuttonalliance.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:26:53 2026 GMT\n  hsts: null\n  note: >-\n    servers[] host of the harvested Green Button Alliance OpenAPI in this repo. Not a\n    Toronto Hydro host.\n- host: torontoonboarding.savagedata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 14:06:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  server: Microsoft-IIS/10.0\n  probed_manually: true\n  note: >-\n    Added by hand because the host is carried as DeveloperPortal/SignUp rather than\n    Website, so the automated host collector did not reach it. This is the third-party\n    Green Button onboarding application Toronto Hydro links to\
  \ from its public Green\n    Button page, operated by its platform vendor Savage Data Systems. It negotiates\n    TLSv1.2 only (no TLSv1.3) and advertises a 30-day HSTS max-age — a weaker posture\n    than Toronto Hydro's own www host, on the surface a developer must actually use.\ndomains:\n- domain: torontohydro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: greenbuttonalliance.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: savagedata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  probed_manually: true\n  note: Platform vendor domain hosting Toronto Hydro's Green Button third-party onboarding application.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/security/toronto-hydro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Canada
- Utilities
- Electricity
- Smart Metering
- Green Button
- Grid
- Ontario
- Consumer Data
- Electricity Distribution
---
