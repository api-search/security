---
api_specs:
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Clients API
  slug: wodify-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Leads API
  slug: wodify-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Memberships API
  slug: wodify-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Classes and Programs API
  slug: wodify-classes-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Workouts and Performance API
  slug: wodify-workouts-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Services and Appointments API
  slug: wodify-services-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Financials API
  slug: wodify-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Communications API
  slug: wodify-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wodify.com
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: api.wodify.com
  hsts: false
  https: true
  note: Documented API base host (https://api.wodify.com/v1). Root path 301-redirects to docs.wodify.com.
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: app-api.wodify.com
  hsts: false
  https: true
  note: Underlying API gateway host shown in the authentication docs example.
  tls_version: TLSv1.3
- cert_expires: Sep 12 21:08:03 2026 GMT
  host: www.wodify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: docs.wodify.com
  https: true
  note: Public documentation host.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wodify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wodify, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wodify
provider_slug: wodify
slug: wodify-domain-security
source_filename: wodify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.wodify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: false\n  note: 'Documented API base host (https://api.wodify.com/v1). Root path 301-redirects to docs.wodify.com.'\n- host: app-api.wodify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: false\n  note: Underlying API gateway host shown in the authentication docs example.\n- host: www.wodify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 21:08:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.wodify.com\n  https: true\n  tls_version: TLSv1.3\n  note: Public documentation host.\ndomains:\n- domain: wodify.com\n  dnssec: false\n  caa:\n  - '0 issue \"pki.goog\"'\n  - '0 issue \"amazon.com\"'\n  - '0 issue \"godaddy.com\"'\n  - '0 issue \"letsencrypt.org\"'\n  spf: true\n  dmarc:\
  \ true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/security/wodify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- Gym Management
- Membership Management
- Fitness Software
- CrossFit
- Class Scheduling
- Billing
- Wellness
- SaaS
---
