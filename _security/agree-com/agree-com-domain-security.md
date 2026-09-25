---
api_specs:
- filename: agree-com-agreements-api-openapi.yml
  format: yaml
  label: Agree.com Agreements API
  slug: agree-com-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-agreements-api-openapi.yml
- filename: agree-com-contacts-api-openapi.yml
  format: yaml
  label: Agree.com Contacts API
  slug: agree-com-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-contacts-api-openapi.yml
- filename: agree-com-customers-api-openapi.yml
  format: yaml
  label: Agree.com Customers API
  slug: agree-com-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-customers-api-openapi.yml
- filename: agree-com-invoices-api-openapi.yml
  format: yaml
  label: Agree.com Invoices API
  slug: agree-com-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-invoices-api-openapi.yml
- filename: agree-com-reports-api-openapi.yml
  format: yaml
  label: Agree.com Reports API
  slug: agree-com-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-reports-api-openapi.yml
- filename: agree-com-webhooks-api-openapi.yml
  format: yaml
  label: Agree.com Webhooks API
  slug: agree-com-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agree.com
  spf: true
hosts:
- cert_expires: Oct 10 11:53:59 2026 GMT
  host: agree.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 10:19:21 2026 GMT
  host: secure.agree.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Agree Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agree.com, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agree.com
provider_slug: agree-com
slug: agree-com-domain-security
source_filename: agree-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agree.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 11:53:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: secure.agree.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 10:19:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agree.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/security/agree-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agreements
- Electronic Signature
- Contract Management
- Invoicing
- Billing
- Payments
- Accounts Receivable
- Fintech
- Financial Services
- Webhook
- MCP
- Agent-Native
---
