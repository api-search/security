---
api_specs:
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Products & Prices API
  slug: products-prices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Checkouts API
  slug: checkouts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Subscriptions API
  slug: subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Benefits & License Keys API
  slug: benefits-license-keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Meters & Events API
  slug: meters-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
- filename: polar-sh-openapi.yml
  format: yaml
  label: Polar Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/openapi/polar-sh-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: polar.sh
  spf: true
hosts:
- cert_expires: Aug 29 20:42:31 2026 GMT
  host: polar.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 04:39:11 2026 GMT
  host: api.polar.sh
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 20:31:04 2026 GMT
  host: sandbox-api.polar.sh
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polar Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Polar
provider_slug: polar-sh
slug: polar-sh-domain-security
source_filename: polar-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polar.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 20:42:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.polar.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 04:39:11 2026 GMT\n  hsts: null\n- host: sandbox-api.polar.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 20:31:04 2026 GMT\n  hsts: null\ndomains:\n- domain: polar.sh\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polar-sh/refs/heads/main/security/polar-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Billing
- Payments
- Merchant of Record
- Monetization
- Subscriptions
- Usage Based Billing
---
