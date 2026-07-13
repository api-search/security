---
api_specs:
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Contacts API
  slug: sevdesk-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Invoices API
  slug: sevdesk-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Orders API
  slug: sevdesk-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Credit Notes API
  slug: sevdesk-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Vouchers API
  slug: sevdesk-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Bank and Transactions API
  slug: sevdesk-bank-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Parts API
  slug: sevdesk-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Tags API
  slug: sevdesk-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Export and Reports API
  slug: sevdesk-export-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sevdesk.de
  nameservers:
  - liv.ns.cloudflare.com
  - frank.ns.cloudflare.com
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:_spf.cmail.ondemand.com include:4999173.spf02.hubspotemail.net -all
hosts:
- cert_expires: Sep 24 01:36:09 2026 GMT
  cert_issuer: Let's Encrypt (CN=YR1)
  host: sevdesk.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 02:24:48 2026 GMT
  cert_issuer: Google Trust Services (CN=WE1)
  host: my.sevdesk.de
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 02:24:48 2026 GMT
  cert_issuer: Google Trust Services (CN=WE1)
  host: api.sevdesk.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sevdesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sevdesk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: sevdesk
provider_slug: sevdesk
slug: sevdesk-domain-security
source_filename: sevdesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sevdesk.de\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt (CN=YR1)\n  cert_expires: Sep 24 01:36:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: my.sevdesk.de\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (CN=WE1)\n  cert_expires: Oct  4 02:24:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n- host: api.sevdesk.de\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (CN=WE1)\n  cert_expires: Oct  4 02:24:48 2026 GMT\n  hsts: false\ndomains:\n- domain: sevdesk.de\n  nameservers:\n  - liv.ns.cloudflare.com\n  - frank.ns.cloudflare.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com include:_spf.cmail.ondemand.com include:4999173.spf02.hubspotemail.net -all\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/security/sevdesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Invoicing
- Bookkeeping
- Finance
- Germany
- Vouchers
- Contacts
- SaaS
- ERP
- Financial Software
---
