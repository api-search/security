---
api_specs:
- filename: hooklogic-criteo-retailmedia-openapi-original.json
  format: json
  label: Criteo Retail Media API
  slug: criteo-retail-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-retailmedia-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: criteo.com
  spf: true
hosts:
- cert_expires: Sep  2 23:59:59 2026 GMT
  host: api.criteo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hooklogic Criteo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HookLogic (Criteo), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HookLogic (Criteo)
provider_slug: hooklogic-criteo
slug: hooklogic-criteo-domain-security
source_filename: hooklogic-criteo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.criteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: criteo.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/security/hooklogic-criteo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- Retail Media
- Advertising
- E-commerce
- Marketing
- Retail
- APIs
---
