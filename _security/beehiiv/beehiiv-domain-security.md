---
api_specs:
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Publications API
  slug: beehiiv-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Subscriptions API
  slug: beehiiv-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Posts API
  slug: beehiiv-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Automations API
  slug: beehiiv-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Custom Fields API
  slug: beehiiv-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Segments API
  slug: beehiiv-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Tiers API
  slug: beehiiv-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Polls API
  slug: beehiiv-polls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Webhooks API
  slug: beehiiv-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Newsletter Lists API
  slug: beehiiv-newsletter-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Referral Program API
  slug: beehiiv-referral-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv OAuth2 API
  slug: beehiiv-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: beehiiv.com
  spf: true
hosts:
- cert_expires: Sep 24 03:10:29 2026 GMT
  host: www.beehiiv.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 03:10:29 2026 GMT
  host: developers.beehiiv.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 03:10:29 2026 GMT
  host: api.beehiiv.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beehiiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for beehiiv, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: beehiiv
provider_slug: beehiiv
slug: beehiiv-domain-security
source_filename: beehiiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beehiiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:10:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.beehiiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:10:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.beehiiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:10:29 2026 GMT\n  hsts: null\ndomains:\n- domain: beehiiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/security/beehiiv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Newsletter
- Creator
- Email
- Subscription
- Publishing
- Media
- Advertising
---
