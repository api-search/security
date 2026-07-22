---
api_specs:
- filename: solvimon-configuration-api-openapi.yml
  format: yaml
  label: Solvimon Configuration API
  slug: solvimon-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/openapi/solvimon-configuration-api-openapi.yml
- filename: solvimon-transaction-api-openapi.yml
  format: yaml
  label: Solvimon Transaction API
  slug: solvimon-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/openapi/solvimon-transaction-api-openapi.yml
- filename: solvimon-identity-api-openapi.yml
  format: yaml
  label: Solvimon Identity API
  slug: solvimon-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/openapi/solvimon-identity-api-openapi.yml
- filename: solvimon-event-api-openapi.yml
  format: yaml
  label: Solvimon Event API
  slug: solvimon-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/openapi/solvimon-event-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: solvimon.com
  spf: true
hosts:
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: www.solvimon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 00:38:04 2026 GMT
  host: test.api.solvimon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 17:30:04 2026 GMT
  host: api.solvimon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solvimon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solvimon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Solvimon
provider_slug: solvimon
slug: solvimon-domain-security
source_filename: solvimon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solvimon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: test.api.solvimon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 00:38:04 2026 GMT\n  hsts: null\n- host: api.solvimon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 17:30:04 2026 GMT\n  hsts: null\ndomains:\n- domain: solvimon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solvimon/refs/heads/main/security/solvimon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Billing
- Payments
- Monetization
- Usage-Based Pricing
- Subscriptions
- Invoicing
- Metering
- Revenue Recognition
---
