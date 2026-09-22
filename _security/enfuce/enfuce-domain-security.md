---
api_specs:
- filename: enfuce-authorisation-request-api-api-openapi.yml
  format: yaml
  label: Enfuce Authorisation Request API
  slug: enfuce-authorisation-request-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-authorisation-request-api-api-openapi.yml
- filename: enfuce-create-card-api-openapi.yml
  format: yaml
  label: Enfuce Create Card API
  slug: enfuce-create-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-create-card-api-openapi.yml
- filename: enfuce-create-pin-control-access-token-api-openapi.yml
  format: yaml
  label: Enfuce Create PIN Control access token API
  slug: enfuce-create-pin-control-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-create-pin-control-access-token-api-openapi.yml
- filename: enfuce-get-card-api-openapi.yml
  format: yaml
  label: Enfuce Get card API
  slug: enfuce-get-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-get-card-api-openapi.yml
- filename: enfuce-get-card-payment-info-api-openapi.yml
  format: yaml
  label: Enfuce Get Card Payment Info API
  slug: enfuce-get-card-payment-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-get-card-payment-info-api-openapi.yml
- filename: enfuce-get-plastic-manufacturing-history-api-openapi.yml
  format: yaml
  label: Enfuce Get plastic manufacturing history API
  slug: enfuce-get-plastic-manufacturing-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-get-plastic-manufacturing-history-api-openapi.yml
- filename: enfuce-update-card-api-openapi.yml
  format: yaml
  label: Enfuce Update card API
  slug: enfuce-update-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-update-card-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: enfuce.com
  spf: true
hosts:
- cert_expires: Nov 22 09:43:11 2026 GMT
  host: enfuce.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Enfuce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enfuce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Enfuce
provider_slug: enfuce
slug: enfuce-domain-security
source_filename: enfuce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enfuce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 09:43:11 2026 GMT\n  hsts: false\ndomains:\n- domain: enfuce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/security/enfuce-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Card Issuing
- FinTech
- API Platform
---
