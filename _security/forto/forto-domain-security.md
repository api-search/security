---
api_specs:
- filename: forto-openapi.yml
  format: yaml
  label: Forto Public API
  slug: forto-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forto/refs/heads/main/openapi/forto-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@forto.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: forto.com
  spf: true
hosts:
- cert_expires: Aug 20 17:31:32 2026 GMT
  host: forto.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 09:17:09 2026 GMT
  host: developers.forto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.forto.com
  https: false
kind: domain-security
layout: security
method: probed
name: Forto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forto, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Forto
provider_slug: forto
slug: forto-domain-security
source_filename: forto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 17:31:32 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.forto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 09:17:09 2026 GMT\n  hsts: null\n- host: api.forto.com\n  https: false\ndomains:\n- domain: forto.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@forto.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forto/refs/heads/main/security/forto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Freight
- Logistics
- Supply Chain
- Shipping
- Freight Forwarding
- EDI
---
