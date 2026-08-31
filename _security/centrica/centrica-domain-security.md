---
api_specs:
- filename: centrica-oauth2-api-openapi.yml
  format: yaml
  label: Centrica Oauth2 API
  slug: centrica-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrica/refs/heads/main/openapi/centrica-oauth2-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: centrica.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: britishgas.co.uk
  spf: true
  spf_policy: softfail
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bordgaisenergy.ie
  spf: true
  spf_policy: fail
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hivehome.com
  spf: true
  spf_policy: softfail
hosts:
- cert_expires: Sep 10 16:56:03 2026 GMT
  host: www.centrica.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 11:18:52 2026 GMT
  host: api-developer.dev.fieldops.centrica.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 11:18:52 2026 GMT
  host: api.dev.fieldops.centrica.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: www.britishgas.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
kind: domain-security
layout: security
method: probed
name: Centrica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centrica, probed live across 4 host(s) and 4 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Centrica
provider_slug: centrica
slug: centrica-domain-security
source_filename: centrica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.centrica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 16:56:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-developer.dev.fieldops.centrica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 11:18:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dev.fieldops.centrica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 11:18:52 2026 GMT\n  hsts: null\n- host: www.britishgas.co.uk\n  https: true\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: centrica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: britishgas.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: softfail\n  dmarc: true\n  dmarc_policy: reject\n- domain: bordgaisenergy.ie\n  dnssec: false\n  caa:\
  \ []\n  spf: true\n  spf_policy: fail\n  dmarc: true\n  dmarc_policy: reject\n- domain: hivehome.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: softfail\n  dmarc: true\n  dmarc_policy: reject\nnotes: >-\n  Added on the 2026-07-27 enrichment round: the British Gas retail host and the three\n  sibling brand domains (britishgas.co.uk, bordgaisenergy.ie, hivehome.com) were probed\n  by hand because they carry the group's public surface but are not apis.yml baseURL hosts.\n  All four registrable domains share the same posture — DMARC p=reject with Valimail\n  aggregate reporting, SPF present, no CAA records published and no DNSSEC. TLS 1.3 and a\n  one-year HSTS max-age on every reachable web host; the FieldOps development gateway\n  (api.dev.fieldops.centrica.com) is the only host that sends no HSTS header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrica/refs/heads/main/security/centrica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Energy Retail
- Energy Markets
- Ireland
- Field Service
---
