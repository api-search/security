---
api_specs:
- filename: brandtrack-accounts-api-openapi.yml
  format: yaml
  label: Brandtrack Accounts API
  slug: brandtrack-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/openapi/brandtrack-accounts-api-openapi.yml
- filename: brandtrack-groups-api-openapi.yml
  format: yaml
  label: Brandtrack Groups API
  slug: brandtrack-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/openapi/brandtrack-groups-api-openapi.yml
- filename: brandtrack-locations-api-openapi.yml
  format: yaml
  label: Brandtrack Locations API
  slug: brandtrack-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/openapi/brandtrack-locations-api-openapi.yml
- filename: brandtrack-other-api-openapi.yml
  format: yaml
  label: Brandtrack Other API
  slug: brandtrack-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/openapi/brandtrack-other-api-openapi.yml
- filename: brandtrack-partner-api-openapi.yml
  format: yaml
  label: Brandtrack Partner API
  slug: brandtrack-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/openapi/brandtrack-partner-api-openapi.yml
- filename: brandtrack-roles-api-openapi.yml
  format: yaml
  label: Brandtrack Roles API
  slug: brandtrack-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/openapi/brandtrack-roles-api-openapi.yml
- filename: brandtrack-subscriptions-api-openapi.yml
  format: yaml
  label: Brandtrack Subscriptions API
  slug: brandtrack-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/openapi/brandtrack-subscriptions-api-openapi.yml
- filename: brandtrack-users-api-openapi.yml
  format: yaml
  label: Brandtrack Users API
  slug: brandtrack-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/openapi/brandtrack-users-api-openapi.yml
- filename: brandtrack-zones-api-openapi.yml
  format: yaml
  label: Brandtrack Zones API
  slug: brandtrack-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/openapi/brandtrack-zones-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brandtrack.fm
  spf: true
hosts:
- cert_expires: Sep 14 05:14:23 2026 GMT
  host: brandtrack.fm
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.brandtrack.fm
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Brandtrack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brandtrack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brandtrack
provider_slug: brandtrack
slug: brandtrack-domain-security
source_filename: brandtrack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brandtrack.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:14:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.brandtrack.fm\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: brandtrack.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/security/brandtrack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Music
- Background Music
- Audio
- Streaming
- Retail
- Hospitality
- In-Store Experience
- Media
- Sound
---
