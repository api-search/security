---
api_specs:
- filename: treasuryspring-calendar-api-openapi.yml
  format: yaml
  label: TreasurySpring Calendar API
  slug: treasuryspring-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-calendar-api-openapi.yml
- filename: treasuryspring-cells-api-openapi.yml
  format: yaml
  label: TreasurySpring Cells API
  slug: treasuryspring-cells-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-cells-api-openapi.yml
- filename: treasuryspring-entities-api-openapi.yml
  format: yaml
  label: TreasurySpring Entities API
  slug: treasuryspring-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-entities-api-openapi.yml
- filename: treasuryspring-event-checkpoints-api-openapi.yml
  format: yaml
  label: TreasurySpring Event Checkpoints API
  slug: treasuryspring-event-checkpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-event-checkpoints-api-openapi.yml
- filename: treasuryspring-events-api-openapi.yml
  format: yaml
  label: TreasurySpring Events API
  slug: treasuryspring-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-events-api-openapi.yml
- filename: treasuryspring-healthcheck-api-openapi.yml
  format: yaml
  label: TreasurySpring Healthcheck API
  slug: treasuryspring-healthcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-healthcheck-api-openapi.yml
- filename: treasuryspring-holdings-api-openapi.yml
  format: yaml
  label: TreasurySpring Holdings API
  slug: treasuryspring-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-holdings-api-openapi.yml
- filename: treasuryspring-indications-api-openapi.yml
  format: yaml
  label: TreasurySpring Indications API
  slug: treasuryspring-indications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-indications-api-openapi.yml
- filename: treasuryspring-oauth-api-openapi.yml
  format: yaml
  label: TreasurySpring OAuth API
  slug: treasuryspring-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-oauth-api-openapi.yml
- filename: treasuryspring-obligor-exposure-api-openapi.yml
  format: yaml
  label: TreasurySpring Obligor Exposure API
  slug: treasuryspring-obligor-exposure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-obligor-exposure-api-openapi.yml
- filename: treasuryspring-subscriptions-api-openapi.yml
  format: yaml
  label: TreasurySpring Subscriptions API
  slug: treasuryspring-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-subscriptions-api-openapi.yml
- filename: treasuryspring-tasks-api-openapi.yml
  format: yaml
  label: TreasurySpring Tasks API
  slug: treasuryspring-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-tasks-api-openapi.yml
- filename: treasuryspring-webhooks-api-openapi.yml
  format: yaml
  label: TreasurySpring Webhooks API
  slug: treasuryspring-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: treasuryspring.com
  spf: true
hosts:
- cert_expires: Sep 17 19:02:52 2026 GMT
  host: www.treasuryspring.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: api.treasuryspring.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: api.sandbox.treasuryspring.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Treasuryspring Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TreasurySpring, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TreasurySpring
provider_slug: treasuryspring
slug: treasuryspring-domain-security
source_filename: treasuryspring-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.treasuryspring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:02:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.treasuryspring.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\n- host: api.sandbox.treasuryspring.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: treasuryspring.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/security/treasuryspring-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Cash Management
- Treasury
- Investments
- Financial-Services
- Fixed Term Funds
- Payments
- MCP
---
