---
api_specs:
- filename: complyadvantage-openapi.yml
  format: yaml
  label: ComplyAdvantage Search API
  slug: complyadvantage-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-openapi.yml
- filename: complyadvantage-openapi.yml
  format: yaml
  label: ComplyAdvantage Monitored Search API
  slug: complyadvantage-monitored-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-openapi.yml
- filename: complyadvantage-openapi.yml
  format: yaml
  label: ComplyAdvantage Case Management API
  slug: complyadvantage-case-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-openapi.yml
- filename: complyadvantage-openapi.yml
  format: yaml
  label: ComplyAdvantage Users API
  slug: complyadvantage-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: complyadvantage.com
  spf: true
hosts:
- cert_expires: Sep 13 08:00:33 2026 GMT
  host: complyadvantage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: docs.complyadvantage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: api.complyadvantage.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Complyadvantage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ComplyAdvantage, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ComplyAdvantage
provider_slug: complyadvantage
slug: complyadvantage-domain-security
source_filename: complyadvantage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: complyadvantage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:00:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.complyadvantage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.complyadvantage.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: complyadvantage.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/security/complyadvantage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Anti-Money Laundering
- AML
- Fraud Detection
- Sanctions Screening
- Compliance
- PEP Screening
- Adverse Media
- KYC
- Watchlists
- Transaction Monitoring
- Financial Crime
- RegTech
---
