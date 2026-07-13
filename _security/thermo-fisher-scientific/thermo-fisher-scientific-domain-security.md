---
api_specs:
- filename: thermo-fisher-samplemanager-openapi.yml
  format: yaml
  label: Thermo Fisher SampleManager LIMS REST API
  slug: samplemanager-lims
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-samplemanager-openapi.yml
- filename: thermo-fisher-nanodrop-openapi.yml
  format: yaml
  label: Thermo Fisher NanoDrop Ultra Web API
  slug: nanodrop-ultra
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-nanodrop-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thermofisher.com
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: www.thermofisher.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: documents.thermofisher.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: api.thermofisher.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thermo Fisher Scientific Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thermo Fisher Scientific, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Thermo Fisher Scientific
provider_slug: thermo-fisher-scientific
slug: thermo-fisher-scientific-domain-security
source_filename: thermo-fisher-scientific-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thermofisher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: documents.thermofisher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: null\n- host: api.thermofisher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: thermofisher.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/security/thermo-fisher-scientific-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Life Sciences
- Laboratory
- Scientific Instruments
- LIMS
- Diagnostics
- Biosciences
- Fortune 500
---
