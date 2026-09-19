---
api_specs:
- filename: geocitation-audits-api-openapi.yml
  format: yaml
  label: GEOCitation Audits API
  slug: geocitation-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/openapi/geocitation-audits-api-openapi.yml
- filename: geocitation-gdpr-api-openapi.yml
  format: yaml
  label: GEOCitation Gdpr API
  slug: geocitation-gdpr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/openapi/geocitation-gdpr-api-openapi.yml
- filename: geocitation-health-api-openapi.yml
  format: yaml
  label: GEOCitation Health API
  slug: geocitation-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/openapi/geocitation-health-api-openapi.yml
- filename: geocitation-meta-api-openapi.yml
  format: yaml
  label: GEOCitation Meta API
  slug: geocitation-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/openapi/geocitation-meta-api-openapi.yml
- filename: geocitation-opt-out-api-openapi.yml
  format: yaml
  label: GEOCitation Opt Out API
  slug: geocitation-opt-out-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/openapi/geocitation-opt-out-api-openapi.yml
- filename: geocitation-usage-api-openapi.yml
  format: yaml
  label: GEOCitation Usage API
  slug: geocitation-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/openapi/geocitation-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geocitation.io
  spf: true
hosts:
- cert_expires: Dec  5 09:00:08 2026 GMT
  host: www.geocitation.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 08:39:52 2026 GMT
  host: api.geocitation.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Geocitation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GEOCitation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GEOCitation
provider_slug: geocitation
slug: geocitation-domain-security
source_filename: geocitation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geocitation.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 09:00:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.geocitation.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 08:39:52 2026 GMT\n  hsts: null\ndomains:\n- domain: geocitation.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/security/geocitation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SEO
- Geo
- AEO
- AI Search Visibility
- Content Intelligence
- Competitive Intelligence
- Marketing
- MarTech
- White Label
- Agency Tooling
- Web Data & Analytics
---
