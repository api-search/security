---
api_specs:
- filename: vincario-openapi.yml
  format: yaml
  label: Vincario VIN Decode API
  slug: vin-decode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-openapi.yml
- filename: vincario-openapi.yml
  format: yaml
  label: Vincario Vehicle Market Value API
  slug: market-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-openapi.yml
- filename: vincario-openapi.yml
  format: yaml
  label: Vincario Stolen Check API
  slug: stolen-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-openapi.yml
- filename: vincario-openapi.yml
  format: yaml
  label: Vincario Vehicle Info API
  slug: vehicle-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-openapi.yml
- filename: vincario-openapi.yml
  format: yaml
  label: Vincario Account Balance API
  slug: account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vincario.com
  spf: true
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: vindecoder.eu
  spf: true
hosts:
- cert_expires: Aug 16 14:58:53 2026 GMT
  host: vincario.com
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 15:00:45 2026 GMT
  host: vindecoder.eu
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 14:58:54 2026 GMT
  host: api.vindecoder.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vincario Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vincario, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Vincario
provider_slug: vincario
slug: vincario-domain-security
source_filename: vincario-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vincario.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 14:58:53 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\n- host: vindecoder.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:00:45 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\n- host: api.vindecoder.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:58:54 2026 GMT\n  hsts: null\ndomains:\n- domain: vincario.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: vindecoder.eu\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/security/vincario-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- VIN
- Vehicle Data
- Automotive
- VIN Decoder
- Market Value
---
