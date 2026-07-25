---
api_specs:
- filename: markforged-builds-api-openapi.yml
  format: yaml
  label: Markforged Builds API
  slug: markforged-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-builds-api-openapi.yml
- filename: markforged-devices-api-openapi.yml
  format: yaml
  label: Markforged Devices API
  slug: markforged-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-devices-api-openapi.yml
- filename: markforged-organizations-api-openapi.yml
  format: yaml
  label: Markforged Organizations API
  slug: markforged-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-organizations-api-openapi.yml
- filename: markforged-parts-api-openapi.yml
  format: yaml
  label: Markforged Parts API
  slug: markforged-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-parts-api-openapi.yml
- filename: markforged-print-jobs-api-openapi.yml
  format: yaml
  label: Markforged Print Jobs API
  slug: markforged-print-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-print-jobs-api-openapi.yml
- filename: markforged-printed-parts-api-openapi.yml
  format: yaml
  label: Markforged Printed Parts API
  slug: markforged-printed-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-printed-parts-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:devops+caa@markforged.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: markforged.com
  spf: true
- caa:
  - 0 issue "starfieldtech.com"
  - 0 iodef "mailto:devops+caa@markforged.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eiger.io
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: markforged.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  5 15:34:19 2027 GMT
  host: www.eiger.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Markforged Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Markforged, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Markforged
provider_slug: markforged
slug: markforged-domain-security
source_filename: markforged-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: markforged.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\n- host: www.eiger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 15:34:19 2027 GMT\n  hsts: null\ndomains:\n- domain: markforged.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:devops+caa@markforged.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: eiger.io\n  dnssec: false\n  caa:\n  - 0 issue \"starfieldtech.com\"\n  - 0 iodef \"mailto:devops+caa@markforged.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/security/markforged-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- 3D Printing
- Additive Manufacturing
- Industrial
- Eiger
- Fleet Management
---
