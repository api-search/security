---
api_specs:
- filename: arthur-online-properties-openapi.yml
  format: yaml
  label: Arthur Properties API
  slug: arthur-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-properties-openapi.yml
- filename: arthur-online-units-openapi.yml
  format: yaml
  label: Arthur Units API
  slug: arthur-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-units-openapi.yml
- filename: arthur-online-tenancies-openapi.yml
  format: yaml
  label: Arthur Tenancies API
  slug: arthur-tenancies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-tenancies-openapi.yml
- filename: arthur-online-tenants-openapi.yml
  format: yaml
  label: Arthur Tenants API
  slug: arthur-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-tenants-openapi.yml
- filename: arthur-online-applicants-openapi.yml
  format: yaml
  label: Arthur Applicants API
  slug: arthur-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-applicants-openapi.yml
- filename: arthur-online-viewings-openapi.yml
  format: yaml
  label: Arthur Viewings API
  slug: arthur-viewings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-viewings-openapi.yml
- filename: arthur-online-maintenance-openapi.yml
  format: yaml
  label: Arthur Maintenance API
  slug: arthur-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-maintenance-openapi.yml
- filename: arthur-online-financials-openapi.yml
  format: yaml
  label: Arthur Financials API
  slug: arthur-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-financials-openapi.yml
- filename: arthur-online-assets-openapi.yml
  format: yaml
  label: Arthur Assets API
  slug: arthur-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-assets-openapi.yml
- filename: arthur-online-utilities-openapi.yml
  format: yaml
  label: Arthur Utilities API
  slug: arthur-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-utilities-openapi.yml
- filename: arthur-online-certificates-openapi.yml
  format: yaml
  label: Arthur Certificates API
  slug: arthur-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-certificates-openapi.yml
- filename: arthur-online-entities-openapi.yml
  format: yaml
  label: Arthur Entities API
  slug: arthur-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-entities-openapi.yml
- filename: arthur-online-conversations-openapi.yml
  format: yaml
  label: Arthur Conversations API
  slug: arthur-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-conversations-openapi.yml
- filename: arthur-online-tags-openapi.yml
  format: yaml
  label: Arthur Tags API
  slug: arthur-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-tags-openapi.yml
- filename: arthur-online-notes-openapi.yml
  format: yaml
  label: Arthur Notes API
  slug: arthur-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-notes-openapi.yml
- filename: arthur-online-types-openapi.yml
  format: yaml
  label: Arthur Types API
  slug: arthur-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-types-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arthuronline.co.uk
  spf: true
hosts:
- cert_expires: Oct  3 21:16:39 2026 GMT
  host: www.arthuronline.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 19:13:50 2026 GMT
  host: developer.arthuronline.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 19:13:50 2026 GMT
  host: api.arthuronline.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arthur Online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arthur Online, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arthur Online
provider_slug: arthur-online
slug: arthur-online-domain-security
source_filename: arthur-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arthuronline.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:16:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.arthuronline.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 19:13:50 2026 GMT\n  hsts: null\n- host: api.arthuronline.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 19:13:50 2026 GMT\n  hsts: null\ndomains:\n- domain: arthuronline.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/security/arthur-online-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- United Kingdom
- Property Management
- PropTech
- Rentals
- Lettings
- Tenancy
- Maintenance
- Property Listings
- Social Housing
- Student Housing
- Block Management
---
