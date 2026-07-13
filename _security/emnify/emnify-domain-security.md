---
api_specs:
- filename: emnify-api-openapi.yml
  format: yaml
  label: emnify REST API
  slug: emnify-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emnify/refs/heads/main/openapi/emnify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emnify.com
  spf: true
- caa:
  - 0 iodef "mailto:steffen.gebert+caa-emnify-net@emnify.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emnify.net
  spf: true
hosts:
- cert_expires: Sep 19 11:55:27 2026 GMT
  host: www.emnify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 19:42:13 2026 GMT
  host: docs.emnify.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: cdn.emnify.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emnify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for emnify, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: emnify
provider_slug: emnify
slug: emnify-domain-security
source_filename: emnify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.emnify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 11:55:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.emnify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 19:42:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cdn.emnify.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: emnify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: emnify.net\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:steffen.gebert+caa-emnify-net@emnify.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emnify/refs/heads/main/security/emnify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Internet of Things
- Cellular Connectivity
- IoT SIM
- eSIM
- Consumer eSIM
- SGP.32
- M2M
- NTN-IoT
- Satellite
- SuperNetwork
---
