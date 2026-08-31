---
api_specs:
- filename: instapage-workspaces-api-openapi.yml
  format: yaml
  label: Instapage Workspaces API
  slug: instapage-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-workspaces-api-openapi.yml
- filename: instapage-analytics-api-openapi.yml
  format: yaml
  label: Instapage Analytics API
  slug: instapage-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-analytics-api-openapi.yml
- filename: instapage-assets-api-openapi.yml
  format: yaml
  label: Instapage Assets API
  slug: instapage-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-assets-api-openapi.yml
- filename: instapage-collections-api-openapi.yml
  format: yaml
  label: Instapage Collections API
  slug: instapage-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-collections-api-openapi.yml
- filename: instapage-domains-api-openapi.yml
  format: yaml
  label: Instapage Domains API
  slug: instapage-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-domains-api-openapi.yml
- filename: instapage-experiments-api-openapi.yml
  format: yaml
  label: Instapage Experiments API
  slug: instapage-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-experiments-api-openapi.yml
- filename: instapage-form-submissions-api-openapi.yml
  format: yaml
  label: Instapage Form Submissions API
  slug: instapage-form-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-form-submissions-api-openapi.yml
- filename: instapage-groups-api-openapi.yml
  format: yaml
  label: Instapage Groups API
  slug: instapage-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-groups-api-openapi.yml
- filename: instapage-pages-api-openapi.yml
  format: yaml
  label: Instapage Pages API
  slug: instapage-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-pages-api-openapi.yml
- filename: instapage-personalizations-api-openapi.yml
  format: yaml
  label: Instapage Personalizations API
  slug: instapage-personalizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-personalizations-api-openapi.yml
- filename: instapage-team-members-api-openapi.yml
  format: yaml
  label: Instapage Team Members API
  slug: instapage-team-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-team-members-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:sysadmins@instapage.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: instapage.com
  spf: true
hosts:
- cert_expires: Oct  6 08:18:16 2026 GMT
  host: instapage.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 08:18:16 2026 GMT
  host: devdocs.instapage.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 08:18:16 2026 GMT
  host: api.instapage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instapage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instapage, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Instapage
provider_slug: instapage
slug: instapage-domain-security
source_filename: instapage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instapage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:18:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: devdocs.instapage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:18:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.instapage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:18:16 2026 GMT\n  hsts: null\ndomains:\n- domain: instapage.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:sysadmins@instapage.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/security/instapage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Landing Pages
- Conversion Optimization
- Marketing
- A/B Testing
- Post-Click Optimization
- Lead Generation
---
