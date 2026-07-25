---
api_specs:
- filename: thumbtack-authentication-api-openapi.yml
  format: yaml
  label: Thumbtack Authentication API
  slug: thumbtack-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-authentication-api-openapi.yml
- filename: thumbtack-autocomplete-api-openapi.yml
  format: yaml
  label: Thumbtack Autocomplete API
  slug: thumbtack-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-autocomplete-api-openapi.yml
- filename: thumbtack-categories-api-openapi.yml
  format: yaml
  label: Thumbtack Categories API
  slug: thumbtack-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-categories-api-openapi.yml
- filename: thumbtack-leads-api-openapi.yml
  format: yaml
  label: Thumbtack Leads API
  slug: thumbtack-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-leads-api-openapi.yml
- filename: thumbtack-messages-api-openapi.yml
  format: yaml
  label: Thumbtack Messages API
  slug: thumbtack-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-messages-api-openapi.yml
- filename: thumbtack-orders-api-openapi.yml
  format: yaml
  label: Thumbtack Orders API
  slug: thumbtack-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-orders-api-openapi.yml
- filename: thumbtack-pro-profiles-api-openapi.yml
  format: yaml
  label: Thumbtack Pro Profiles API
  slug: thumbtack-pro-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-pro-profiles-api-openapi.yml
- filename: thumbtack-pros-api-openapi.yml
  format: yaml
  label: Thumbtack Pros API
  slug: thumbtack-pros-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-pros-api-openapi.yml
- filename: thumbtack-reviews-api-openapi.yml
  format: yaml
  label: Thumbtack Reviews API
  slug: thumbtack-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-reviews-api-openapi.yml
- filename: thumbtack-testing-api-openapi.yml
  format: yaml
  label: Thumbtack Testing API
  slug: thumbtack-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-testing-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thumbtack.com
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.thumbtack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: developers.thumbtack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.thumbtack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thumbtack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thumbtack, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Thumbtack
provider_slug: thumbtack
slug: thumbtack-domain-security
source_filename: thumbtack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thumbtack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\n- host: developers.thumbtack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.thumbtack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: thumbtack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/security/thumbtack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Local Services
- Marketplace
- Home Services
- Leads
- Partner API
---
