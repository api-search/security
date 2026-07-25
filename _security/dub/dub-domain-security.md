---
api_specs:
- filename: dub-analytics-api-openapi.yml
  format: yaml
  label: Dub Analytics API
  slug: dub-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-analytics-api-openapi.yml
- filename: dub-bounties-api-openapi.yml
  format: yaml
  label: Dub Bounties API
  slug: dub-bounties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-bounties-api-openapi.yml
- filename: dub-commissions-api-openapi.yml
  format: yaml
  label: Dub Commissions API
  slug: dub-commissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-commissions-api-openapi.yml
- filename: dub-customers-api-openapi.yml
  format: yaml
  label: Dub Customers API
  slug: dub-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-customers-api-openapi.yml
- filename: dub-domains-api-openapi.yml
  format: yaml
  label: Dub Domains API
  slug: dub-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-domains-api-openapi.yml
- filename: dub-embed-tokens-api-openapi.yml
  format: yaml
  label: Dub Embed Tokens API
  slug: dub-embed-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-embed-tokens-api-openapi.yml
- filename: dub-events-api-openapi.yml
  format: yaml
  label: Dub Events API
  slug: dub-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-events-api-openapi.yml
- filename: dub-folders-api-openapi.yml
  format: yaml
  label: Dub Folders API
  slug: dub-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-folders-api-openapi.yml
- filename: dub-links-api-openapi.yml
  format: yaml
  label: Dub Links API
  slug: dub-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-links-api-openapi.yml
- filename: dub-partner-applications-api-openapi.yml
  format: yaml
  label: Dub Partner Applications API
  slug: dub-partner-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-partner-applications-api-openapi.yml
- filename: dub-partners-api-openapi.yml
  format: yaml
  label: Dub Partners API
  slug: dub-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-partners-api-openapi.yml
- filename: dub-payouts-api-openapi.yml
  format: yaml
  label: Dub Payouts API
  slug: dub-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-payouts-api-openapi.yml
- filename: dub-qr-codes-api-openapi.yml
  format: yaml
  label: Dub QR Codes API
  slug: dub-qr-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-qr-codes-api-openapi.yml
- filename: dub-tags-api-openapi.yml
  format: yaml
  label: Dub Tags API
  slug: dub-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-tags-api-openapi.yml
- filename: dub-track-api-openapi.yml
  format: yaml
  label: Dub Track API
  slug: dub-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-track-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dub.co
  spf: true
hosts:
- cert_expires: Sep 22 13:01:56 2026 GMT
  host: dub.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 13:01:56 2026 GMT
  host: api.dub.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dub, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dub
provider_slug: dub
slug: dub-domain-security
source_filename: dub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dub.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:01:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.dub.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:01:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dub.co\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/security/dub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Link Management
- URL Shortener
- Analytics
- Conversion Tracking
- Affiliate Programs
- Open Source
---
