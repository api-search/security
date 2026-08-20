---
api_specs:
- filename: simplifi-simplifipay-auth-api-openapi.yml
  format: yaml
  label: Simplifi/Simplifipay Auth API
  slug: simplifi-simplifipay-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/openapi/simplifi-simplifipay-auth-api-openapi.yml
- filename: simplifi-simplifipay-card-api-openapi.yml
  format: yaml
  label: Simplifi/Simplifipay Card API
  slug: simplifi-simplifipay-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/openapi/simplifi-simplifipay-card-api-openapi.yml
- filename: simplifi-simplifipay-card-program-api-openapi.yml
  format: yaml
  label: Simplifi/Simplifipay Card Program API
  slug: simplifi-simplifipay-card-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/openapi/simplifi-simplifipay-card-program-api-openapi.yml
- filename: simplifi-simplifipay-document-api-openapi.yml
  format: yaml
  label: Simplifi/Simplifipay Document API
  slug: simplifi-simplifipay-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/openapi/simplifi-simplifipay-document-api-openapi.yml
- filename: simplifi-simplifipay-fee-api-openapi.yml
  format: yaml
  label: Simplifi/Simplifipay Fee API
  slug: simplifi-simplifipay-fee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/openapi/simplifi-simplifipay-fee-api-openapi.yml
- filename: simplifi-simplifipay-funding-source-api-openapi.yml
  format: yaml
  label: Simplifi/Simplifipay Funding Source API
  slug: simplifi-simplifipay-funding-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/openapi/simplifi-simplifipay-funding-source-api-openapi.yml
- filename: simplifi-simplifipay-transaction-api-openapi.yml
  format: yaml
  label: Simplifi/Simplifipay Transaction API
  slug: simplifi-simplifipay-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/openapi/simplifi-simplifipay-transaction-api-openapi.yml
- filename: simplifi-simplifipay-user-api-openapi.yml
  format: yaml
  label: Simplifi/Simplifipay User API
  slug: simplifi-simplifipay-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/openapi/simplifi-simplifipay-user-api-openapi.yml
- filename: simplifi-simplifipay-webhook-api-openapi.yml
  format: yaml
  label: Simplifi/Simplifipay Webhook API
  slug: simplifi-simplifipay-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/openapi/simplifi-simplifipay-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simplifipay.com
  spf: true
hosts:
- cert_expires: Sep 15 09:42:45 2026 GMT
  host: simplifipay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simplifi Simplifipay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simplifi/Simplifipay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Simplifi/Simplifipay
provider_slug: simplifi-simplifipay
slug: simplifi-simplifipay-domain-security
source_filename: simplifi-simplifipay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simplifipay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:42:45 2026 GMT\n  hsts: false\ndomains:\n- domain: simplifipay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/security/simplifi-simplifipay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cards
- Card Issuing
- Virtual Cards
- Fintech
- Payments
- Banking as a Service
- Embedded Finance
- GCC
- Webhook
---
