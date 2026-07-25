---
api_specs:
- filename: oracle-retail-fulfillment-api-openapi.yml
  format: yaml
  label: Oracle Retail Fulfillment API
  slug: oracle-retail-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-fulfillment-api-openapi.yml
- filename: oracle-retail-inventory-api-openapi.yml
  format: yaml
  label: Oracle Retail Inventory API
  slug: oracle-retail-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-inventory-api-openapi.yml
- filename: oracle-retail-items-api-openapi.yml
  format: yaml
  label: Oracle Retail Items API
  slug: oracle-retail-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-items-api-openapi.yml
- filename: oracle-retail-orders-api-openapi.yml
  format: yaml
  label: Oracle Retail Orders API
  slug: oracle-retail-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-orders-api-openapi.yml
- filename: oracle-retail-purchaseorders-api-openapi.yml
  format: yaml
  label: Oracle Retail PurchaseOrders API
  slug: oracle-retail-purchaseorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-purchaseorders-api-openapi.yml
- filename: oracle-retail-returns-api-openapi.yml
  format: yaml
  label: Oracle Retail Returns API
  slug: oracle-retail-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-returns-api-openapi.yml
- filename: oracle-retail-suppliers-api-openapi.yml
  format: yaml
  label: Oracle Retail Suppliers API
  slug: oracle-retail-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-suppliers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.oracle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Retail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Retail, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Retail
provider_slug: oracle-retail
slug: oracle-retail-domain-security
source_filename: oracle-retail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: www.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/security/oracle-retail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Merchandising
- Order Management
- Pricing
- Inventory
- Point of Sale
- Omnichannel
- Oracle
---
