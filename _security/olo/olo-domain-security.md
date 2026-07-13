---
api_specs:
- filename: olo-ordering-openapi.yml
  format: yaml
  label: Olo Ordering API
  slug: olo-ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/openapi/olo-ordering-openapi.yml
- filename: olo-ordering-openapi.yml
  format: yaml
  label: Olo Rails API
  slug: olo-rails
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/openapi/olo-ordering-openapi.yml
- filename: olo-promotions-openapi.yml
  format: yaml
  label: Olo Loyalty API
  slug: olo-loyalty
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/openapi/olo-promotions-openapi.yml
- filename: olo-webhooks-asyncapi.yml
  format: yaml
  label: Olo Webhooks
  slug: olo-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/asyncapi/olo-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: olo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zendesk.com
  spf: true
hosts:
- cert_expires: Sep 13 05:08:50 2026 GMT
  host: www.olo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 19:59:23 2026 GMT
  host: developer.olo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 08:06:26 2026 GMT
  host: olosupport.zendesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Olo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Olo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Olo
provider_slug: olo
slug: olo-domain-security
source_filename: olo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.olo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 05:08:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.olo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:59:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: olosupport.zendesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:06:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: olo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zendesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/security/olo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food Service
- Restaurants
- Online Ordering
- Delivery
- Point of Sale
- Hospitality
- Payments
- Loyalty
- Marketing
---
