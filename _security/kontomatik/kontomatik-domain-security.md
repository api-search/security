---
api_specs:
- filename: kontomatik-aggregation-api-openapi.yml
  format: yaml
  label: Kontomatik Aggregation API
  slug: kontomatik-aggregation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-aggregation-api-openapi.yml
- filename: kontomatik-catalog-api-openapi.yml
  format: yaml
  label: Kontomatik Catalog API
  slug: kontomatik-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-catalog-api-openapi.yml
- filename: kontomatik-command-api-openapi.yml
  format: yaml
  label: Kontomatik Command API
  slug: kontomatik-command-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-command-api-openapi.yml
- filename: kontomatik-confirmations-api-openapi.yml
  format: yaml
  label: Kontomatik Confirmations API
  slug: kontomatik-confirmations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-confirmations-api-openapi.yml
- filename: kontomatik-features-api-openapi.yml
  format: yaml
  label: Kontomatik Features API
  slug: kontomatik-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-features-api-openapi.yml
- filename: kontomatik-income-api-openapi.yml
  format: yaml
  label: Kontomatik Income API
  slug: kontomatik-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-income-api-openapi.yml
- filename: kontomatik-labeling-api-openapi.yml
  format: yaml
  label: Kontomatik Labeling API
  slug: kontomatik-labeling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-labeling-api-openapi.yml
- filename: kontomatik-mock-api-openapi.yml
  format: yaml
  label: Kontomatik Mock API
  slug: kontomatik-mock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-mock-api-openapi.yml
- filename: kontomatik-owner-api-openapi.yml
  format: yaml
  label: Kontomatik Owner API
  slug: kontomatik-owner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-owner-api-openapi.yml
- filename: kontomatik-profile-api-openapi.yml
  format: yaml
  label: Kontomatik Profile API
  slug: kontomatik-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-profile-api-openapi.yml
- filename: kontomatik-reports-api-openapi.yml
  format: yaml
  label: Kontomatik Reports API
  slug: kontomatik-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-reports-api-openapi.yml
- filename: kontomatik-score-api-openapi.yml
  format: yaml
  label: Kontomatik Score API
  slug: kontomatik-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-score-api-openapi.yml
- filename: kontomatik-signin-api-openapi.yml
  format: yaml
  label: Kontomatik SignIn API
  slug: kontomatik-signin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-signin-api-openapi.yml
- filename: kontomatik-statements-api-openapi.yml
  format: yaml
  label: Kontomatik Statements API
  slug: kontomatik-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-statements-api-openapi.yml
- filename: kontomatik-summary-api-openapi.yml
  format: yaml
  label: Kontomatik Summary API
  slug: kontomatik-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-summary-api-openapi.yml
- filename: kontomatik-vendors-api-openapi.yml
  format: yaml
  label: Kontomatik Vendors API
  slug: kontomatik-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-vendors-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kontomatik.com
  spf: true
hosts:
- cert_expires: Oct  8 15:52:18 2026 GMT
  host: kontomatik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 03:01:18 2026 GMT
  host: developer.kontomatik.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 18:39:22 2026 GMT
  host: api.kontomatik.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kontomatik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kontomatik, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kontomatik
provider_slug: kontomatik
slug: kontomatik-domain-security
source_filename: kontomatik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kontomatik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 15:52:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.kontomatik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 03:01:18 2026 GMT\n  hsts: false\n- host: api.kontomatik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:39:22 2026 GMT\n  hsts: null\ndomains:\n- domain: kontomatik.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/security/kontomatik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Banking
- PSD2
- AIS
- Bank Data Aggregation
- CEE
- KYC
- Credit Scoring
- Transaction Labeling
- PDF Parsing
---
