---
api_specs:
- filename: cardlytics-partner-api-openapi.yml
  format: yaml
  label: Cardlytics Partner API
  slug: cardlytics-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-partner-api-openapi.yml
- filename: cardlytics-campaign-build-api-openapi.yml
  format: yaml
  label: Cardlytics Campaign Build API
  slug: cardlytics-campaign-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-campaign-build-api-openapi.yml
- filename: cardlytics-publisher-api-openapi.yml
  format: yaml
  label: Cardlytics Publisher API v2
  slug: cardlytics-publisher-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-publisher-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "trust-provider.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cardlytics.com
  spf: true
hosts:
- cert_expires: Oct 27 04:58:14 2026 GMT
  host: www.cardlytics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: api-sandbox.cardlytics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: api.cardlytics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cardlytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardlytics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cardlytics
provider_slug: cardlytics
slug: cardlytics-domain-security
source_filename: cardlytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cardlytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 04:58:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-sandbox.cardlytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: null\n- host: api.cardlytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cardlytics.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"trust-provider.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/security/cardlytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Commerce Media
- Card-Linked Offers
- Purchase Intelligence
- Financial-Services
- Loyalty and Rewards
- Marketing
- Banking
- Retail Media
- Attribution
- Offers
---
