---
api_specs:
- filename: messente-account-balance-api-openapi.yml
  format: yaml
  label: Messente Account Balance API
  slug: messente-account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-account-balance-api-openapi.yml
- filename: messente-blacklist-api-openapi.yml
  format: yaml
  label: Messente Blacklist API
  slug: messente-blacklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-blacklist-api-openapi.yml
- filename: messente-bulk-messaging-api-openapi.yml
  format: yaml
  label: Messente Bulk Messaging API
  slug: messente-bulk-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-bulk-messaging-api-openapi.yml
- filename: messente-contacts-api-openapi.yml
  format: yaml
  label: Messente Contacts API
  slug: messente-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-contacts-api-openapi.yml
- filename: messente-delivery-report-api-openapi.yml
  format: yaml
  label: Messente Delivery Report API
  slug: messente-delivery-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-delivery-report-api-openapi.yml
- filename: messente-groups-api-openapi.yml
  format: yaml
  label: Messente Groups API
  slug: messente-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-groups-api-openapi.yml
- filename: messente-number-lookup-api-openapi.yml
  format: yaml
  label: Messente Number Lookup API
  slug: messente-number-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-number-lookup-api-openapi.yml
- filename: messente-number-verification-api-openapi.yml
  format: yaml
  label: Messente Number Verification API
  slug: messente-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-number-verification-api-openapi.yml
- filename: messente-omnimessage-api-openapi.yml
  format: yaml
  label: Messente Omnimessage API
  slug: messente-omnimessage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-omnimessage-api-openapi.yml
- filename: messente-pricing-api-openapi.yml
  format: yaml
  label: Messente Pricing API
  slug: messente-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-pricing-api-openapi.yml
- filename: messente-statistics-api-openapi.yml
  format: yaml
  label: Messente Statistics API
  slug: messente-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-statistics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: messente.com
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: messente.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: api.messente.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Messente Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Messente, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Messente
provider_slug: messente
slug: messente-domain-security
source_filename: messente-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: messente.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\n- host: api.messente.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: messente.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/security/messente-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- CPaaS
- Messaging
- SMS
- Viber
- WhatsApp
- Verification
- 2FA
---
