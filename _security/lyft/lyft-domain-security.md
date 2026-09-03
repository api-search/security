---
api_specs:
- filename: lyft-concierge-rides-api-openapi.yml
  format: yaml
  label: lyft Concierge Rides API
  slug: lyft-concierge-rides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-concierge-rides-api-openapi.yml
- filename: lyft-cost-estimates-api-openapi.yml
  format: yaml
  label: lyft Cost Estimates API
  slug: lyft-cost-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-cost-estimates-api-openapi.yml
- filename: lyft-drivers-api-openapi.yml
  format: yaml
  label: lyft Drivers API
  slug: lyft-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-drivers-api-openapi.yml
- filename: lyft-eta-api-openapi.yml
  format: yaml
  label: lyft ETA API
  slug: lyft-eta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-eta-api-openapi.yml
- filename: lyft-profile-api-openapi.yml
  format: yaml
  label: lyft Profile API
  slug: lyft-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-profile-api-openapi.yml
- filename: lyft-ride-types-api-openapi.yml
  format: yaml
  label: lyft Ride Types API
  slug: lyft-ride-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-ride-types-api-openapi.yml
- filename: lyft-rides-api-openapi.yml
  format: yaml
  label: lyft Rides API
  slug: lyft-rides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-rides-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "www.digicert.com"
  - 0 iodef "mailto:security@lyft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lyft.com
  spf: true
hosts:
- host: developer.lyft.com
  https: false
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.lyft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: www.lyft.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lyft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lyft, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lyft
provider_slug: lyft
slug: lyft-domain-security
source_filename: lyft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.lyft.com\n  https: false\n- host: api.lyft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\n- host: www.lyft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: lyft.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"www.digicert.com\"\n  - 0 iodef \"mailto:security@lyft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/security/lyft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
