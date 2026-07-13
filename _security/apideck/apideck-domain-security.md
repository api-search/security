---
api_specs:
- filename: apideck-accounting-openapi.yml
  format: yaml
  label: Apideck Accounting API
  slug: accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apideck/refs/heads/main/openapi/apideck-accounting-openapi.yml
- filename: apideck-crm-openapi.yml
  format: yaml
  label: Apideck CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apideck/refs/heads/main/openapi/apideck-crm-openapi.yml
- filename: apideck-hris-openapi.yml
  format: yaml
  label: Apideck HRIS API
  slug: hris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apideck/refs/heads/main/openapi/apideck-hris-openapi.yml
- filename: ats.yml
  format: yaml
  label: Apideck ATS API
  slug: ats-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/ats.yml
- filename: apideck-file-storage-openapi.yml
  format: yaml
  label: Apideck File Storage API
  slug: file-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apideck/refs/heads/main/openapi/apideck-file-storage-openapi.yml
- filename: ecommerce.yml
  format: yaml
  label: Apideck Ecommerce API
  slug: ecommerce-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/ecommerce.yml
- filename: pos.yml
  format: yaml
  label: Apideck POS API
  slug: pos-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/pos.yml
- filename: issue-tracking.yml
  format: yaml
  label: Apideck Issue Tracking API
  slug: issue-tracking-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/issue-tracking.yml
- filename: lead.yml
  format: yaml
  label: Apideck Lead API
  slug: lead-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/lead.yml
- filename: sms.yml
  format: yaml
  label: Apideck SMS API
  slug: sms-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/sms.yml
- filename: vault.yml
  format: yaml
  label: Apideck Vault API
  slug: vault-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/vault.yml
- filename: webhook.yml
  format: yaml
  label: Apideck Webhook API
  slug: webhook-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/webhook.yml
- filename: connector.yml
  format: yaml
  label: Apideck Connector API
  slug: connector-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/connector.yml
- filename: proxy.yml
  format: yaml
  label: Apideck Proxy API
  slug: proxy-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/proxy.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apideck.com
  spf: true
hosts:
- cert_expires: Sep 29 16:52:27 2026 GMT
  host: www.apideck.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: unify.apideck.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:17:12 2026 GMT
  host: developers.apideck.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apideck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apideck, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apideck
provider_slug: apideck
slug: apideck-domain-security
source_filename: apideck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apideck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:52:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: unify.apideck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\n- host: developers.apideck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:17:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: apideck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apideck/refs/heads/main/security/apideck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Integrations
- Unified API
---
