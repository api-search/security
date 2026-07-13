---
api_specs:
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Awards Search API
  slug: usaspending-awards-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Agency API
  slug: usaspending-agency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Recipient API
  slug: usaspending-recipient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Federal Account API
  slug: usaspending-federal-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Budget Function API
  slug: usaspending-budget-function-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Disaster/Emergency Funding (COVID-19) API
  slug: usaspending-disaster-emergency-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Bulk Download API
  slug: usaspending-bulk-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending References & Autocomplete API
  slug: usaspending-references-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Subawards API
  slug: usaspending-subawards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usaspending.gov
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: www.usaspending.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api.usaspending.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Usaspending Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for USAspending.gov, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: USAspending.gov
provider_slug: usaspending
slug: usaspending-domain-security
source_filename: usaspending-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usaspending.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usaspending.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usaspending.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/security/usaspending-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Government
- Federal Spending
- Open Data
- Contracts
- Grants
- DATA Act
- Transparency
- Public Sector
---
