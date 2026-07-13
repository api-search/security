---
api_specs:
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Devices API
  slug: eiger-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Builds API
  slug: eiger-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Print Jobs API
  slug: eiger-print-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Parts API
  slug: eiger-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Printed Parts API
  slug: eiger-printed-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Organizations API
  slug: eiger-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
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
