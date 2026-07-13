---
api_specs:
- filename: grubhub-menu-openapi.yml
  format: yaml
  label: Grubhub Menu API
  slug: menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-menu-openapi.yml
- filename: grubhub-orders-openapi.yml
  format: yaml
  label: Grubhub Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-orders-openapi.yml
- filename: grubhub-merchant-data-openapi.yml
  format: yaml
  label: Grubhub Merchant Data API
  slug: merchant-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-data-openapi.yml
- filename: grubhub-merchant-schedules-openapi.yml
  format: yaml
  label: Grubhub Merchant Schedules API
  slug: merchant-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-schedules-openapi.yml
- filename: grubhub-deliveries-openapi.yml
  format: yaml
  label: Grubhub Deliveries API
  slug: deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-deliveries-openapi.yml
- filename: grubhub-onboarding-openapi.yml
  format: yaml
  label: Grubhub Onboarding API
  slug: onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-onboarding-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: grubhub.com
  spf: true
hosts:
- cert_expires: Nov 24 01:08:20 2026 GMT
  host: developer.grubhub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.grubhub.com
  https: false
- cert_expires: Nov 24 01:08:20 2026 GMT
  host: api-third-party-gtm.grubhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grubhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for grubhub, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: grubhub
provider_slug: grubhub
slug: grubhub-domain-security
source_filename: grubhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.grubhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 01:08:20 2026 GMT\n  hsts: false\n- host: api.grubhub.com\n  https: false\n- host: api-third-party-gtm.grubhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 01:08:20 2026 GMT\n  hsts: null\ndomains:\n- domain: grubhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/security/grubhub-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags: []
---
