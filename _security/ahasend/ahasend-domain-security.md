---
api_specs:
- filename: ahasend-accounts-api-openapi.yml
  format: yaml
  label: AhaSend Accounts API
  slug: ahasend-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-accounts-api-openapi.yml
- filename: ahasend-api-keys-api-openapi.yml
  format: yaml
  label: AhaSend API Keys API
  slug: ahasend-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-api-keys-api-openapi.yml
- filename: ahasend-domains-api-openapi.yml
  format: yaml
  label: AhaSend Domains API
  slug: ahasend-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-domains-api-openapi.yml
- filename: ahasend-email-api-openapi.yml
  format: yaml
  label: AhaSend Email API
  slug: ahasend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-email-api-openapi.yml
- filename: ahasend-messages-api-openapi.yml
  format: yaml
  label: AhaSend Messages API
  slug: ahasend-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-messages-api-openapi.yml
- filename: ahasend-routes-api-openapi.yml
  format: yaml
  label: AhaSend Routes API
  slug: ahasend-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-routes-api-openapi.yml
- filename: ahasend-smtp-credentials-api-openapi.yml
  format: yaml
  label: AhaSend SMTP Credentials API
  slug: ahasend-smtp-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-smtp-credentials-api-openapi.yml
- filename: ahasend-statistics-api-openapi.yml
  format: yaml
  label: AhaSend Statistics API
  slug: ahasend-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-statistics-api-openapi.yml
- filename: ahasend-suppressions-api-openapi.yml
  format: yaml
  label: AhaSend Suppressions API
  slug: ahasend-suppressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-suppressions-api-openapi.yml
- filename: ahasend-utility-api-openapi.yml
  format: yaml
  label: AhaSend Utility API
  slug: ahasend-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-utility-api-openapi.yml
- filename: ahasend-webhooks-api-openapi.yml
  format: yaml
  label: AhaSend Webhooks API
  slug: ahasend-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ahasend.com
  spf: true
hosts:
- cert_expires: Aug 19 15:55:34 2026 GMT
  host: ahasend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 09:30:23 2026 GMT
  host: api.ahasend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ahasend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AhaSend, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AhaSend
provider_slug: ahasend
slug: ahasend-domain-security
source_filename: ahasend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ahasend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 15:55:34 2026 GMT\n  hsts: false\n- host: api.ahasend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 09:30:23 2026 GMT\n  hsts: null\ndomains:\n- domain: ahasend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/security/ahasend-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhook
---
