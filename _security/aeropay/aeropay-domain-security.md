---
api_specs:
- filename: aeropay-authentication-api-openapi.yml
  format: yaml
  label: Aeropay Authentication API
  slug: aeropay-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeropay/refs/heads/main/openapi/aeropay-authentication-api-openapi.yml
- filename: aeropay-bank-connection-api-openapi.yml
  format: yaml
  label: Aeropay Bank Connection API
  slug: aeropay-bank-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeropay/refs/heads/main/openapi/aeropay-bank-connection-api-openapi.yml
- filename: aeropay-create-manage-transactions-api-openapi.yml
  format: yaml
  label: Aeropay Create & Manage Transactions API
  slug: aeropay-create-manage-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeropay/refs/heads/main/openapi/aeropay-create-manage-transactions-api-openapi.yml
- filename: aeropay-merchant-management-api-openapi.yml
  format: yaml
  label: Aeropay Merchant Management API
  slug: aeropay-merchant-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeropay/refs/heads/main/openapi/aeropay-merchant-management-api-openapi.yml
- filename: aeropay-reports-api-openapi.yml
  format: yaml
  label: Aeropay Reports API
  slug: aeropay-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeropay/refs/heads/main/openapi/aeropay-reports-api-openapi.yml
- filename: aeropay-user-management-api-openapi.yml
  format: yaml
  label: Aeropay User Management API
  slug: aeropay-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeropay/refs/heads/main/openapi/aeropay-user-management-api-openapi.yml
- filename: aeropay-webhooks-api-openapi.yml
  format: yaml
  label: Aeropay Webhooks API
  slug: aeropay-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeropay/refs/heads/main/openapi/aeropay-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aeropay.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: aero.inc
  spf: false
hosts:
- cert_expires: Nov 19 05:42:25 2026 GMT
  host: www.aeropay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 04:13:17 2026 GMT
  host: dev.aero.inc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: api.aeropay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aeropay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aeropay, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Aeropay
provider_slug: aeropay
slug: aeropay-domain-security
source_filename: aeropay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aeropay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 05:42:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.aero.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 04:13:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.aeropay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: aeropay.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: aero.inc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeropay/refs/heads/main/security/aeropay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Pay by Bank
- ACH
- Open Banking
- Fintech
- Bank linking
- Financial-Services
- Real-Time Payments
- Webhook
- Payouts
- MCP
- Risk & fraud
---
