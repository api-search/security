---
api_specs:
- filename: fedex-openapi.yml
  format: yaml
  label: FedEx Track API
  slug: track
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fedex/refs/heads/main/openapi/fedex-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "identrust.com"
  - 0 iodef "mailto:hostmaster@fedex.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fedex.com
  spf: true
hosts:
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: www.fedex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: developer.fedex.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: apis.fedex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fedex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FedEx, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FedEx
provider_slug: fedex
slug: fedex-domain-security
source_filename: fedex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fedex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: null\n- host: developer.fedex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: apis.fedex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fedex.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"identrust.com\"\n  - 0 iodef \"mailto:hostmaster@fedex.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fedex/refs/heads/main/security/fedex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Address Validation
- Freight
- Logistics
- Pickup
- Rating
- Shipping
- Tracking
- Webhooks
- Fortune 100
---
