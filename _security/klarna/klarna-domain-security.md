---
api_specs:
- filename: klarna-payments-api-openapi.yml
  format: yaml
  label: Klarna Payments API
  slug: klarna-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-payments-api-openapi.yml
- filename: klarna-customer-token-api-openapi.yml
  format: yaml
  label: Klarna Customer Token API
  slug: klarna-customer-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-customer-token-api-openapi.yml
- filename: klarna-settlements-api-openapi.yml
  format: yaml
  label: Klarna Settlements API
  slug: klarna-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-settlements-api-openapi.yml
- filename: klarna-push-notifications-asyncapi.yml
  format: yaml
  label: Klarna Push Notifications
  slug: klarna-push-notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/asyncapi/klarna-push-notifications-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "amazonaws.com"
  - 0 iodef "mailto:dns-admin@klarna.com"
  - 0 issue "e-szigno.hu"
  - 0 issue "buypass.no"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: klarna.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: www.klarna.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: docs.klarna.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.klarna.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Klarna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klarna, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Klarna
provider_slug: klarna
slug: klarna-domain-security
source_filename: klarna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.klarna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.klarna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.klarna.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: klarna.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 iodef \"mailto:dns-admin@klarna.com\"\n  - 0 issue \"e-szigno.hu\"\n  - 0 issue \"buypass.no\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/security/klarna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- BNPL
- Payments
- Cards
- Shopping
---
