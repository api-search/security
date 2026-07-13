---
api_specs:
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto People / Contacts API
  slug: people-contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Custom Activities API
  slug: custom-activities
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Campaigns API
  slug: campaigns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Tags API
  slug: tags
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Transactional Email API
  slug: transactional-email
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ortto.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ap3api.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: ortto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: help.ortto.com
  https: false
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: api.ap3api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ortto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ortto, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ortto
provider_slug: ortto
slug: ortto-domain-security
source_filename: ortto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ortto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.ortto.com\n  https: false\n- host: api.ap3api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ortto.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ap3api.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/security/ortto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Marketing Automation
- CDP
- Customer Data Platform
- Analytics
- Email
---
