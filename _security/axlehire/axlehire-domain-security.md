---
api_specs:
- filename: axlehire-assignment-information-api-openapi.yml
  format: yaml
  label: AxleHire (Jitsu) Assignment Information API
  slug: axlehire-assignment-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axlehire/refs/heads/main/openapi/axlehire-assignment-information-api-openapi.yml
- filename: axlehire-driver-information-api-openapi.yml
  format: yaml
  label: AxleHire (Jitsu) Driver Information API
  slug: axlehire-driver-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axlehire/refs/heads/main/openapi/axlehire-driver-information-api-openapi.yml
- filename: axlehire-partner-information-api-openapi.yml
  format: yaml
  label: AxleHire (Jitsu) Partner Information API
  slug: axlehire-partner-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axlehire/refs/heads/main/openapi/axlehire-partner-information-api-openapi.yml
- filename: axlehire-shipping-information-api-openapi.yml
  format: yaml
  label: AxleHire (Jitsu) Shipping Information API
  slug: axlehire-shipping-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axlehire/refs/heads/main/openapi/axlehire-shipping-information-api-openapi.yml
- filename: axlehire-tracking-information-api-openapi.yml
  format: yaml
  label: AxleHire (Jitsu) Tracking Information API
  slug: axlehire-tracking-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axlehire/refs/heads/main/openapi/axlehire-tracking-information-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gojitsu.com
  spf: true
hosts:
- cert_expires: Sep 16 00:45:07 2026 GMT
  host: gojitsu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 15:38:57 2026 GMT
  host: docs.gojitsu.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 01:54:41 2026 GMT
  host: api.gojitsu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axlehire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AxleHire (Jitsu), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AxleHire (Jitsu)
provider_slug: axlehire
slug: axlehire-domain-security
source_filename: axlehire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gojitsu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 00:45:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.gojitsu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 15:38:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.gojitsu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 01:54:41 2026 GMT\n  hsts: null\ndomains:\n- domain: gojitsu.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axlehire/refs/heads/main/security/axlehire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Logistics
- Last Mile Delivery
- Shipping
- Parcel
- Transportation
- Supply Chain
- E-Commerce
- Tracking
- Webhook
---
