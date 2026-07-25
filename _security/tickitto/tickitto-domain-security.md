---
api_specs:
- filename: tickitto-authentication-api-openapi.yml
  format: yaml
  label: Tickitto Authentication API
  slug: tickitto-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-authentication-api-openapi.yml
- filename: tickitto-availability-api-openapi.yml
  format: yaml
  label: Tickitto Availability API
  slug: tickitto-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-availability-api-openapi.yml
- filename: tickitto-basket-api-openapi.yml
  format: yaml
  label: Tickitto Basket API
  slug: tickitto-basket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-basket-api-openapi.yml
- filename: tickitto-events-api-openapi.yml
  format: yaml
  label: Tickitto Events API
  slug: tickitto-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-events-api-openapi.yml
- filename: tickitto-metadata-api-openapi.yml
  format: yaml
  label: Tickitto Metadata API
  slug: tickitto-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-metadata-api-openapi.yml
- filename: tickitto-search-api-openapi.yml
  format: yaml
  label: Tickitto Search API
  slug: tickitto-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-search-api-openapi.yml
- filename: tickitto-system-status-api-openapi.yml
  format: yaml
  label: Tickitto System Status API
  slug: tickitto-system-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-system-status-api-openapi.yml
- filename: tickitto-webhooks-api-openapi.yml
  format: yaml
  label: Tickitto Webhooks API
  slug: tickitto-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tickitto.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tickitto.tech
  spf: true
hosts:
- cert_expires: Sep 19 21:51:12 2026 GMT
  host: tickitto.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 01:33:42 2026 GMT
  host: docs.tickitto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 12:13:12 2026 GMT
  host: tickitto.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tickitto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tickitto, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tickitto
provider_slug: tickitto
slug: tickitto-domain-security
source_filename: tickitto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tickitto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:51:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.tickitto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 01:33:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tickitto.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 12:13:12 2026 GMT\n  hsts: null\ndomains:\n- domain: tickitto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tickitto.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/security/tickitto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ticketing
- Events
- Marketplace
- Travel & Experiences
- Entertainment
- Payments
- Commerce
---
