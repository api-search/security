---
api_specs:
- filename: reputation-asset-library-api-openapi.yml
  format: yaml
  label: Reputation Asset Library API
  slug: reputation-asset-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-asset-library-api-openapi.yml
- filename: reputation-authorize-api-openapi.yml
  format: yaml
  label: Reputation Authorize API
  slug: reputation-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-authorize-api-openapi.yml
- filename: reputation-categories-api-openapi.yml
  format: yaml
  label: Reputation Categories API
  slug: reputation-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-categories-api-openapi.yml
- filename: reputation-credentials-api-openapi.yml
  format: yaml
  label: Reputation Credentials API
  slug: reputation-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-credentials-api-openapi.yml
- filename: reputation-listing-audits-api-openapi.yml
  format: yaml
  label: Reputation Listing Audits API
  slug: reputation-listing-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-listing-audits-api-openapi.yml
- filename: reputation-locations-api-openapi.yml
  format: yaml
  label: Reputation Locations API
  slug: reputation-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-locations-api-openapi.yml
- filename: reputation-metrics-api-openapi.yml
  format: yaml
  label: Reputation Metrics API
  slug: reputation-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-metrics-api-openapi.yml
- filename: reputation-reports-api-openapi.yml
  format: yaml
  label: Reputation Reports API
  slug: reputation-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-reports-api-openapi.yml
- filename: reputation-requests-api-openapi.yml
  format: yaml
  label: Reputation Requests API
  slug: reputation-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-requests-api-openapi.yml
- filename: reputation-reviews-api-openapi.yml
  format: yaml
  label: Reputation Reviews API
  slug: reputation-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-reviews-api-openapi.yml
- filename: reputation-rich-content-api-openapi.yml
  format: yaml
  label: Reputation Rich Content API
  slug: reputation-rich-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-rich-content-api-openapi.yml
- filename: reputation-summary-api-openapi.yml
  format: yaml
  label: Reputation Summary API
  slug: reputation-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-summary-api-openapi.yml
- filename: reputation-surveys-api-openapi.yml
  format: yaml
  label: Reputation Surveys API
  slug: reputation-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-surveys-api-openapi.yml
- filename: reputation-tenants-api-openapi.yml
  format: yaml
  label: Reputation Tenants API
  slug: reputation-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-tenants-api-openapi.yml
- filename: reputation-tickets-api-openapi.yml
  format: yaml
  label: Reputation Tickets API
  slug: reputation-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-tickets-api-openapi.yml
- filename: reputation-users-api-openapi.yml
  format: yaml
  label: Reputation Users API
  slug: reputation-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reputation.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: reputation-api.com
  spf: false
hosts:
- cert_expires: Sep 15 20:47:22 2026 GMT
  host: reputation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 09:29:22 2026 GMT
  host: apidocs.reputation.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: reputation-api.com
  https: false
kind: domain-security
layout: security
method: probed
name: Reputation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reputation, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reputation
provider_slug: reputation
slug: reputation-domain-security
source_filename: reputation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reputation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 20:47:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.reputation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 09:29:22 2026 GMT\n  hsts: null\n- host: reputation-api.com\n  https: false\ndomains:\n- domain: reputation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: reputation-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/security/reputation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Reputation Management
- Online Reviews
- Business Listings
- Surveys
- Social Listening
- Competitive Intelligence
- Customer Experience
- Local SEO
---
