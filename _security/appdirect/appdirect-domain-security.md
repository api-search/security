---
api_specs:
- filename: appdirect-companies-openapi-original.yml
  format: yaml
  label: AppDirect Companies / Marketplace API
  slug: appdirect-companies-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdirect/refs/heads/main/openapi/appdirect-companies-openapi-original.yml
- filename: appdirect-devsai-openapi-original.json
  format: json
  label: AppDirect Devs.ai API
  slug: appdirect-devsai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdirect/refs/heads/main/openapi/appdirect-devsai-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:web.master@appdirect.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appdirect.com
  spf: true
hosts:
- cert_expires: Aug 29 23:54:36 2026 GMT
  host: www.appdirect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appdirect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppDirect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AppDirect
provider_slug: appdirect
slug: appdirect-domain-security
source_filename: appdirect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.appdirect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:54:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appdirect.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:web.master@appdirect.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appdirect/refs/heads/main/security/appdirect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- Subscription Commerce
- Marketplace
- Billing
- Reseller
- Cloud Distribution
- Webhooks
- OAuth
---
