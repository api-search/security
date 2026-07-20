---
api_specs:
- filename: currencycloud-openapi-original.yml
  format: yaml
  label: Currencycloud API v2
  slug: currencycloud-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencycloud/refs/heads/main/openapi/currencycloud-openapi-original.yml
- filename: currencycloud-onboarding-openapi-original.yml
  format: yaml
  label: Currencycloud Onboarding API (beta pilot)
  slug: currencycloud-onboarding-api-beta-pilot
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencycloud/refs/heads/main/openapi/currencycloud-onboarding-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issue "visa.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: currencycloud.com
  spf: true
hosts:
- cert_expires: Aug 24 14:57:13 2026 GMT
  host: currencycloud.com
  hsts: true
  hsts_max_age: 264310
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 14:57:13 2026 GMT
  host: api.currencycloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 14:57:13 2026 GMT
  host: devapi.currencycloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Currencycloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Currencycloud, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Currencycloud
provider_slug: currencycloud
slug: currencycloud-domain-security
source_filename: currencycloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: currencycloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:57:13 2026 GMT\n  hsts: true\n  hsts_max_age: 264310\n- host: api.currencycloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:57:13 2026 GMT\n  hsts: null\n- host: devapi.currencycloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:57:13 2026 GMT\n  hsts: null\ndomains:\n- domain: currencycloud.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"visa.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/currencycloud/refs/heads/main/security/currencycloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Payments
- Foreign Exchange
- Cross-Border Payments
- Money Transfer
- Currency Conversion
- Banking
---
