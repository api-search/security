---
api_specs:
- filename: hydro-ottawa-applicationinformation-api-openapi.yml
  format: yaml
  label: Hydro Ottawa Application Information API
  slug: hydro-ottawa-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/openapi/hydro-ottawa-applicationinformation-api-openapi.yml
- filename: hydro-ottawa-authorization-api-openapi.yml
  format: yaml
  label: Hydro Ottawa Authorization API
  slug: hydro-ottawa-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/openapi/hydro-ottawa-authorization-api-openapi.yml
- filename: hydro-ottawa-batch-api-openapi.yml
  format: yaml
  label: Hydro Ottawa Batch API
  slug: hydro-ottawa-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/openapi/hydro-ottawa-batch-api-openapi.yml
- filename: hydro-ottawa-usagepoint-api-openapi.yml
  format: yaml
  label: Hydro Ottawa Usage Point API
  slug: hydro-ottawa-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/openapi/hydro-ottawa-usagepoint-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hydroottawa.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: hydroottawagroup.com
  spf: true
hosts:
- cert_expires: Oct  2 21:49:34 2026 GMT
  host: hydroottawa.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 02:42:41 2026 GMT
  host: hydroottawagroup.com
  hsts: true
  hsts_max_age: 63072000
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
name: Hydro Ottawa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hydro Ottawa, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hydro Ottawa
provider_slug: hydro-ottawa
slug: hydro-ottawa-domain-security
source_filename: hydro-ottawa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hydroottawa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:49:34 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: hydroottawagroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 02:42:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sandbox.greenbuttonalliance.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:26:53 2026 GMT\n  hsts: null\ndomains:\n- domain: hydroottawa.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: hydroottawagroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/security/hydro-ottawa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Canada
- Ontario
- Utilities
- Electricity
- Electricity Distribution
- Smart Metering
- Green Button
- ESPI
- Municipal Utility
- Renewables
- Hydroelectric
- Solar
- Demand Response
- Grid
---
