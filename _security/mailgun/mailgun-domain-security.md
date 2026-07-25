---
api_specs:
- filename: mailgun-domains-api-openapi.yml
  format: yaml
  label: Mailgun Domains API
  slug: mailgun-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-domains-api-openapi.yml
- filename: mailgun-events-api-openapi.yml
  format: yaml
  label: Mailgun Events API
  slug: mailgun-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-events-api-openapi.yml
- filename: mailgun-mailing-lists-api-openapi.yml
  format: yaml
  label: Mailgun Mailing Lists API
  slug: mailgun-mailing-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-mailing-lists-api-openapi.yml
- filename: mailgun-messages-api-openapi.yml
  format: yaml
  label: Mailgun Messages API
  slug: mailgun-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-messages-api-openapi.yml
- filename: mailgun-routes-api-openapi.yml
  format: yaml
  label: Mailgun Routes API
  slug: mailgun-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-routes-api-openapi.yml
- filename: mailgun-suppressions-api-openapi.yml
  format: yaml
  label: Mailgun Suppressions API
  slug: mailgun-suppressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-suppressions-api-openapi.yml
- filename: mailgun-webhooks-api-openapi.yml
  format: yaml
  label: Mailgun Webhooks API
  slug: mailgun-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailgun.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailgun.net
  spf: true
hosts:
- cert_expires: Aug 25 07:03:07 2026 GMT
  host: www.mailgun.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:38:27 2026 GMT
  host: documentation.mailgun.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: api.mailgun.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mailgun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailgun, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mailgun
provider_slug: mailgun
slug: mailgun-domain-security
source_filename: mailgun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mailgun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 07:03:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: documentation.mailgun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:38:27 2026 GMT\n  hsts: false\n- host: api.mailgun.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mailgun.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mailgun.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/security/mailgun-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Transactional Email
- SMTP
- Email Validation
- Email Delivery
- Messaging
---
