---
api_specs:
- filename: bexio-accounting-api-openapi.yml
  format: yaml
  label: bexio Accounting API
  slug: bexio-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-accounting-api-openapi.yml
- filename: bexio-banking-api-openapi.yml
  format: yaml
  label: bexio Banking API
  slug: bexio-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-banking-api-openapi.yml
- filename: bexio-contacts-api-openapi.yml
  format: yaml
  label: bexio Contacts API
  slug: bexio-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-contacts-api-openapi.yml
- filename: bexio-files-api-openapi.yml
  format: yaml
  label: bexio Files API
  slug: bexio-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-files-api-openapi.yml
- filename: bexio-items-api-openapi.yml
  format: yaml
  label: bexio Items API
  slug: bexio-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-items-api-openapi.yml
- filename: bexio-payroll-api-openapi.yml
  format: yaml
  label: bexio Payroll API
  slug: bexio-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-payroll-api-openapi.yml
- filename: bexio-projects-api-openapi.yml
  format: yaml
  label: bexio Projects API
  slug: bexio-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-projects-api-openapi.yml
- filename: bexio-purchase-api-openapi.yml
  format: yaml
  label: bexio Purchase API
  slug: bexio-purchase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-purchase-api-openapi.yml
- filename: bexio-sales-orders-api-openapi.yml
  format: yaml
  label: bexio Sales Orders API
  slug: bexio-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-sales-orders-api-openapi.yml
description: ''
domains:
- domain: bexio.com
  security_txt: true
  security_txt_url: https://www.bexio.com/.well-known/security.txt
hosts:
- host: www.bexio.com
  https: true
- cert_expires: Oct  8 04:42:36 2026 GMT
  host: api.bexio.com
  https: true
  note: Probed 2026-07-17 -> HTTP 401 (Bearer auth required), confirming a live authenticated REST host.
  tls_version: TLSv1.3
- host: auth.bexio.com
  https: true
  note: Keycloak OpenID Connect realm (realms/bexio); openid-configuration served over HTTPS.
- host: docs.bexio.com
  https: true
kind: domain-security
layout: security
method: probed
name: Bexio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bexio, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: bexio
provider_slug: bexio
slug: bexio-domain-security
source_filename: bexio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + API/auth hosts\nhosts:\n- host: www.bexio.com\n  https: true\n- host: api.bexio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:42:36 2026 GMT\n  note: Probed 2026-07-17 -> HTTP 401 (Bearer auth required), confirming a live authenticated REST host.\n- host: auth.bexio.com\n  https: true\n  note: Keycloak OpenID Connect realm (realms/bexio); openid-configuration served over HTTPS.\n- host: docs.bexio.com\n  https: true\ndomains:\n- domain: bexio.com\n  security_txt: true\n  security_txt_url: https://www.bexio.com/.well-known/security.txt\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/security/bexio-domain-security.yml
summary_line: TLSv1.3
tags:
- Accounting
- ERP
- Invoicing
- SMB
- Switzerland
---
