---
api_specs:
- filename: dealhub-quote-api-openapi.yml
  format: yaml
  label: DealHub Quote API
  slug: dealhub-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-quote-api-openapi.yml
- filename: dealhub-headless-api-openapi.yml
  format: yaml
  label: DealHub Headless Quote API
  slug: dealhub-headless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-headless-api-openapi.yml
- filename: dealhub-crm-api-openapi.yml
  format: yaml
  label: DealHub CRM API
  slug: dealhub-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-crm-api-openapi.yml
- filename: dealhub-crm-import-api-openapi.yml
  format: yaml
  label: DealHub CRM Import API
  slug: dealhub-crm-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-crm-import-api-openapi.yml
- filename: dealhub-user-api-openapi.yml
  format: yaml
  label: DealHub User API
  slug: dealhub-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-user-api-openapi.yml
- filename: dealhub-partner-api-openapi.yml
  format: yaml
  label: DealHub Partner API
  slug: dealhub-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-partner-api-openapi.yml
- filename: dealhub-pricing-api-openapi.yml
  format: yaml
  label: DealHub Pricing API
  slug: dealhub-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-pricing-api-openapi.yml
- filename: dealhub-version-api-openapi.yml
  format: yaml
  label: DealHub Version API
  slug: dealhub-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-version-api-openapi.yml
- filename: dealhub-subskribe-api-openapi.yml
  format: yaml
  label: DealHub Subskribe API
  slug: dealhub-subskribe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-subskribe-api-openapi.yml
- filename: dealhub-external-query-openapi.yml
  format: yaml
  label: DealHub External Query (inbound callback contract)
  slug: dealhub-external-query
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-external-query-openapi.yml
- filename: dealhub-callout-api-openapi.yml
  format: yaml
  label: DealHub Callout API (inbound callback contract)
  slug: dealhub-callout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/openapi/dealhub-callout-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dealhub.io
  spf: true
hosts:
- cert_expires: Oct  7 21:47:47 2026 GMT
  host: dealhub.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 08:46:33 2026 GMT
  host: developers.dealhub.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: api.dealhub.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dealhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DealHub, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DealHub
provider_slug: dealhub
slug: dealhub-domain-security
source_filename: dealhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dealhub.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:47:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.dealhub.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 08:46:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dealhub.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dealhub.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealhub/refs/heads/main/security/dealhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CPQ
- Quote-to-Cash
- Contract Lifecycle Management
- Subscription Management
- Billing
- Revenue Operations
- Sales
- Pricing
- Usage-Based Billing
- Revenue Recognition
- Sales Enablement
---
