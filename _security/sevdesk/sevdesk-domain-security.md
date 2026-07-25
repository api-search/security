---
api_specs:
- filename: sevdesk-checkaccount-api-openapi.yml
  format: yaml
  label: sevdesk CheckAccount API
  slug: sevdesk-checkaccount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-checkaccount-api-openapi.yml
- filename: sevdesk-checkaccounttransaction-api-openapi.yml
  format: yaml
  label: sevdesk CheckAccountTransaction API
  slug: sevdesk-checkaccounttransaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-checkaccounttransaction-api-openapi.yml
- filename: sevdesk-contact-api-openapi.yml
  format: yaml
  label: sevdesk Contact API
  slug: sevdesk-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-contact-api-openapi.yml
- filename: sevdesk-creditnote-api-openapi.yml
  format: yaml
  label: sevdesk CreditNote API
  slug: sevdesk-creditnote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-creditnote-api-openapi.yml
- filename: sevdesk-invoice-api-openapi.yml
  format: yaml
  label: sevdesk Invoice API
  slug: sevdesk-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-invoice-api-openapi.yml
- filename: sevdesk-order-api-openapi.yml
  format: yaml
  label: sevdesk Order API
  slug: sevdesk-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-order-api-openapi.yml
- filename: sevdesk-part-api-openapi.yml
  format: yaml
  label: sevdesk Part API
  slug: sevdesk-part-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-part-api-openapi.yml
- filename: sevdesk-tag-api-openapi.yml
  format: yaml
  label: sevdesk Tag API
  slug: sevdesk-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-tag-api-openapi.yml
- filename: sevdesk-voucher-api-openapi.yml
  format: yaml
  label: sevdesk Voucher API
  slug: sevdesk-voucher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-voucher-api-openapi.yml
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
