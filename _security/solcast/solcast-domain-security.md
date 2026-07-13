---
api_specs:
- filename: solcast-openapi.yml
  format: yaml
  label: Solcast API
  slug: solcast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solcast/refs/heads/main/openapi/solcast-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@solcast.com.au"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: solcast.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: solcast.com.au
  spf: true
hosts:
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: solcast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 00:07:44 2026 GMT
  host: docs.solcast.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: api.solcast.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solcast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solcast, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Solcast
provider_slug: solcast
slug: solcast-domain-security
source_filename: solcast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: solcast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.solcast.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 00:07:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.solcast.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: solcast.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@solcast.com.au\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: solcast.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solcast/refs/heads/main/security/solcast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Solar
- Energy
- Forecasting
- Irradiance
- Weather
- Renewable Energy
- PV Power
---
