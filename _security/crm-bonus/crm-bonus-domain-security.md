---
api_specs:
- filename: crm-bonus-auth-api-openapi.yml
  format: yaml
  label: CRM Bonus Auth API
  slug: crm-bonus-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-auth-api-openapi.yml
- filename: crm-bonus-blocked-api-openapi.yml
  format: yaml
  label: CRM Bonus Blocked API
  slug: crm-bonus-blocked-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-blocked-api-openapi.yml
- filename: crm-bonus-cashback-api-openapi.yml
  format: yaml
  label: CRM Bonus Cashback API
  slug: crm-bonus-cashback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-cashback-api-openapi.yml
- filename: crm-bonus-customers-api-openapi.yml
  format: yaml
  label: CRM Bonus Customers API
  slug: crm-bonus-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-customers-api-openapi.yml
- filename: crm-bonus-nps-api-openapi.yml
  format: yaml
  label: CRM Bonus Nps API
  slug: crm-bonus-nps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-nps-api-openapi.yml
- filename: crm-bonus-order-items-api-openapi.yml
  format: yaml
  label: CRM Bonus Order Items API
  slug: crm-bonus-order-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-order-items-api-openapi.yml
- filename: crm-bonus-orders-api-openapi.yml
  format: yaml
  label: CRM Bonus Orders API
  slug: crm-bonus-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-orders-api-openapi.yml
- filename: crm-bonus-products-api-openapi.yml
  format: yaml
  label: CRM Bonus Products API
  slug: crm-bonus-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-products-api-openapi.yml
- filename: crm-bonus-sellers-api-openapi.yml
  format: yaml
  label: CRM Bonus Sellers API
  slug: crm-bonus-sellers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-sellers-api-openapi.yml
- filename: crm-bonus-stores-api-openapi.yml
  format: yaml
  label: CRM Bonus Stores API
  slug: crm-bonus-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-stores-api-openapi.yml
- filename: crm-bonus-tag-hits-api-openapi.yml
  format: yaml
  label: CRM Bonus Tag Hits API
  slug: crm-bonus-tag-hits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-tag-hits-api-openapi.yml
- filename: crm-bonus-tag-ids-api-openapi.yml
  format: yaml
  label: CRM Bonus Tag Ids API
  slug: crm-bonus-tag-ids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-tag-ids-api-openapi.yml
- filename: crm-bonus-tag-interactions-api-openapi.yml
  format: yaml
  label: CRM Bonus Tag Interactions API
  slug: crm-bonus-tag-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-tag-interactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crmbonus.com.br
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: otocrm.com.br
  spf: true
hosts:
- cert_expires: Oct 15 14:32:16 2026 GMT
  host: crmbonus.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 02:20:41 2026 GMT
  host: data-api.otocrm.com.br
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: 'Corrected by hand after the automated pass recorded hsts: null. The probe''s request path returns 404 on this host and the header was missed; a live HEAD on https://data-api.otocrm.com.br/ and on /docs both return "strict-transport-security: max-age=31536000; includeSubDomains" (re-verified 2026-08-12). Fronted by Cloudflare.'
  tls_version: TLSv1.3
- cert_expires: Oct 23 02:20:41 2026 GMT
  host: data-api-hmg.otocrm.com.br
  hsts: null
  https: true
  note: staging (homologação) host; HSTS not confirmed.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crm Bonus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CRM Bonus, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CRM Bonus
provider_slug: crm-bonus
slug: crm-bonus-domain-security
source_filename: crm-bonus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crmbonus.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 14:32:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data-api.otocrm.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 02:20:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    Corrected by hand after the automated pass recorded hsts: null. The probe's\n    request path returns 404 on this host and the header was missed; a live\n    HEAD on https://data-api.otocrm.com.br/ and on /docs both return\n    \"strict-transport-security: max-age=31536000; includeSubDomains\"\n    (re-verified 2026-08-12). Fronted by Cloudflare.\n- host: data-api-hmg.otocrm.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 02:20:41 2026 GMT\n  hsts: null\n  note: staging (homologação) host; HSTS not confirmed.\n\
  domains:\n- domain: crmbonus.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: otocrm.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/security/crm-bonus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Loyalty
- Cashback
- CRM
- Retail Media
- E-Commerce
- Brazil
- WhatsApp
- Customer Data
- Data Ingestion
- Point-of-Sale
---
