---
api_specs:
- filename: balena-openapi.yml
  format: yaml
  label: Balena Cloud API
  slug: balena-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/balena/refs/heads/main/openapi/balena-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: balena.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: balena-cloud.com
  spf: false
hosts:
- cert_expires: Aug 12 21:13:07 2026 GMT
  host: www.balena.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 04:50:17 2026 GMT
  host: docs.balena.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 21:26:56 2026 GMT
  host: api.balena-cloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Balena Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Balena, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Balena
provider_slug: balena
slug: balena-domain-security
source_filename: balena-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.balena.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 21:13:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.balena.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:50:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.balena-cloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 21:26:56 2026 GMT\n  hsts: null\ndomains:\n- domain: balena.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: balena-cloud.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/balena/refs/heads/main/security/balena-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Containers
- Device Management
- Edge
- Embedded Linux
- Fleet Management
- IoT
- OTA
- Provisioning
- Releases
---
