---
api_specs:
- filename: hostbill-accounts-api-openapi.yml
  format: yaml
  label: HostBill Accounts API
  slug: hostbill-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-accounts-api-openapi.yml
- filename: hostbill-admin-api-openapi.yml
  format: yaml
  label: HostBill Admin API
  slug: hostbill-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-admin-api-openapi.yml
- filename: hostbill-clients-api-openapi.yml
  format: yaml
  label: HostBill Clients API
  slug: hostbill-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-clients-api-openapi.yml
- filename: hostbill-domains-api-openapi.yml
  format: yaml
  label: HostBill Domains API
  slug: hostbill-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-domains-api-openapi.yml
- filename: hostbill-invoices-api-openapi.yml
  format: yaml
  label: HostBill Invoices API
  slug: hostbill-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-invoices-api-openapi.yml
- filename: hostbill-orders-api-openapi.yml
  format: yaml
  label: HostBill Orders API
  slug: hostbill-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-orders-api-openapi.yml
- filename: hostbill-tickets-api-openapi.yml
  format: yaml
  label: HostBill Tickets API
  slug: hostbill-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-tickets-api-openapi.yml
- filename: hostbill-transactions-api-openapi.yml
  format: yaml
  label: HostBill Transactions API
  slug: hostbill-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hostbillapp.com
  spf: true
hosts:
- cert_expires: Sep 20 16:46:21 2026 GMT
  host: hostbillapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 16:46:21 2026 GMT
  host: api2.hostbillapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: yourinstance.hostbillapp.com
  https: false
kind: domain-security
layout: security
method: probed
name: Hostbill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HostBill, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HostBill
provider_slug: hostbill
slug: hostbill-domain-security
source_filename: hostbill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hostbillapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 16:46:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api2.hostbillapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 16:46:21 2026 GMT\n  hsts: false\n- host: yourinstance.hostbillapp.com\n  https: false\ndomains:\n- domain: hostbillapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/security/hostbill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Billing
- Domain Registration
- Web Hosting
---
