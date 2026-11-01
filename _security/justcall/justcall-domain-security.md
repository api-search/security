---
api_specs:
- filename: justcall-calls-api-openapi.yml
  format: yaml
  label: JustCall Calls API
  slug: justcall-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-calls-api-openapi.yml
- filename: justcall-contacts-api-openapi.yml
  format: yaml
  label: JustCall Contacts API
  slug: justcall-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-contacts-api-openapi.yml
- filename: justcall-sms-api-openapi.yml
  format: yaml
  label: JustCall SMS API
  slug: justcall-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-sms-api-openapi.yml
- filename: justcall-ai-voice-agents-api-openapi.yml
  format: yaml
  label: JustCall AI Voice Agents API
  slug: justcall-ai-voice-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-ai-voice-agents-api-openapi.yml
- filename: justcall-appointments-api-openapi.yml
  format: yaml
  label: JustCall Appointments API
  slug: justcall-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-appointments-api-openapi.yml
- filename: justcall-justcall-ai-api-openapi.yml
  format: yaml
  label: JustCall JustCall AI API
  slug: justcall-justcall-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-justcall-ai-api-openapi.yml
- filename: justcall-oauth-api-openapi.yml
  format: yaml
  label: JustCall OAuth API
  slug: justcall-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-oauth-api-openapi.yml
- filename: justcall-phone-numbers-api-openapi.yml
  format: yaml
  label: JustCall Phone Numbers API
  slug: justcall-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-phone-numbers-api-openapi.yml
- filename: justcall-rcs-api-openapi.yml
  format: yaml
  label: JustCall RCS API
  slug: justcall-rcs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-rcs-api-openapi.yml
- filename: justcall-sales-dialer-api-openapi.yml
  format: yaml
  label: JustCall Sales Dialer API
  slug: justcall-sales-dialer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-sales-dialer-api-openapi.yml
- filename: justcall-sales-dialer-phone-numbers-api-openapi.yml
  format: yaml
  label: JustCall Sales Dialer - Phone Numbers API
  slug: justcall-sales-dialer-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-sales-dialer-phone-numbers-api-openapi.yml
- filename: justcall-special-dates-api-openapi.yml
  format: yaml
  label: JustCall Special Dates API
  slug: justcall-special-dates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-special-dates-api-openapi.yml
- filename: justcall-unified-analytics-api-openapi.yml
  format: yaml
  label: JustCall Unified Analytics API
  slug: justcall-unified-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-unified-analytics-api-openapi.yml
- filename: justcall-user-groups-api-openapi.yml
  format: yaml
  label: JustCall User Groups API
  slug: justcall-user-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-user-groups-api-openapi.yml
- filename: justcall-users-api-openapi.yml
  format: yaml
  label: JustCall Users API
  slug: justcall-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-users-api-openapi.yml
- filename: justcall-webhooks-api-openapi.yml
  format: yaml
  label: JustCall Webhooks API
  slug: justcall-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-webhooks-api-openapi.yml
- filename: justcall-whats-app-api-openapi.yml
  format: yaml
  label: JustCall Whats App API
  slug: justcall-whats-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-whats-app-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: justcall.io
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: justcall.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 03:28:12 2026 GMT
  host: developer.justcall.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.justcall.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Justcall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JustCall, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JustCall
provider_slug: justcall
slug: justcall-domain-security
source_filename: justcall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justcall.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.justcall.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 03:28:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.justcall.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: justcall.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/justcall/security/justcall-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Voice
- SMS
- Cloud Phone
- Contact Center
- Telephony
- Communications
---
