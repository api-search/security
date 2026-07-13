---
api_specs:
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Authorize / Connect API
  slug: flinks-authorize-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Accounts Detail API
  slug: flinks-accounts-detail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Accounts Summary API
  slug: flinks-accounts-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Statements API
  slug: flinks-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Identity API
  slug: flinks-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Attributes / Analytics API
  slug: flinks-attributes-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Score API
  slug: flinks-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Fraud / KYC API
  slug: flinks-fraud-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flinks.com
  spf: true
hosts:
- cert_expires: Sep  2 22:58:31 2026 GMT
  host: flinks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 16:01:19 2026 GMT
  host: docs.flinks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flinks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flinks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flinks
provider_slug: flinks
slug: flinks-domain-security
source_filename: flinks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flinks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 22:58:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.flinks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 16:01:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: flinks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/security/flinks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Data
- Open Banking
- Bank Aggregation
- Fintech
- Canada
---
