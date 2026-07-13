---
api_specs:
- filename: flexport-openapi.yml
  format: yaml
  label: Flexport REST API
  slug: flexport-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexport/refs/heads/main/openapi/flexport-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "Digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flexport.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.flexport.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 04:05:31 2026 GMT
  host: apidocs.flexport.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: api.flexport.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Flexport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flexport, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flexport
provider_slug: flexport
slug: flexport-domain-security
source_filename: flexport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flexport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.flexport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:05:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.flexport.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: flexport.com\n  dnssec: false\n  caa:\n  - 0 issue \"Digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexport/refs/heads/main/security/flexport-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Freight
- Supply Chain
- Customs
- B2B
---
