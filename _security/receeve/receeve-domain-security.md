---
api_specs:
- filename: receeve-account-api-openapi.yml
  format: yaml
  label: Receeve Account API
  slug: receeve-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-account-api-openapi.yml
- filename: receeve-accountmandate-api-openapi.yml
  format: yaml
  label: Receeve AccountMandate API
  slug: receeve-accountmandate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-accountmandate-api-openapi.yml
- filename: receeve-claim-api-openapi.yml
  format: yaml
  label: Receeve Claim API
  slug: receeve-claim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-claim-api-openapi.yml
- filename: receeve-customtriggers-api-openapi.yml
  format: yaml
  label: Receeve CustomTriggers API
  slug: receeve-customtriggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-customtriggers-api-openapi.yml
- filename: receeve-debtor-api-openapi.yml
  format: yaml
  label: Receeve Debtor API
  slug: receeve-debtor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-debtor-api-openapi.yml
- filename: receeve-event-api-openapi.yml
  format: yaml
  label: Receeve Event API
  slug: receeve-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-event-api-openapi.yml
- filename: receeve-files-api-openapi.yml
  format: yaml
  label: Receeve Files API
  slug: receeve-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-files-api-openapi.yml
- filename: receeve-finance-instalments-v2-api-openapi.yml
  format: yaml
  label: Receeve Finance Instalments V2 API
  slug: receeve-finance-instalments-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-finance-instalments-v2-api-openapi.yml
- filename: receeve-finance-settlements-api-openapi.yml
  format: yaml
  label: Receeve Finance Settlements API
  slug: receeve-finance-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-finance-settlements-api-openapi.yml
- filename: receeve-journey-api-openapi.yml
  format: yaml
  label: Receeve Journey API
  slug: receeve-journey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-journey-api-openapi.yml
- filename: receeve-landingpage-api-openapi.yml
  format: yaml
  label: Receeve LandingPage API
  slug: receeve-landingpage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-landingpage-api-openapi.yml
- filename: receeve-message-api-openapi.yml
  format: yaml
  label: Receeve Message API
  slug: receeve-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-message-api-openapi.yml
- filename: receeve-promisetopay-api-openapi.yml
  format: yaml
  label: Receeve PromiseToPay API
  slug: receeve-promisetopay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-promisetopay-api-openapi.yml
- filename: receeve-security-api-openapi.yml
  format: yaml
  label: Receeve Security API
  slug: receeve-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-security-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: receeve.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: receive-demo.com
  spf: false
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.receeve.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.receive-demo.com
  https: false
kind: domain-security
layout: security
method: probed
name: Receeve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Receeve, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Receeve
provider_slug: receeve
slug: receeve-domain-security
source_filename: receeve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.receeve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\n- host: api.receive-demo.com\n  https: false\ndomains:\n- domain: receeve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: receive-demo.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/security/receeve-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Debt Collection
- Receivables Management
- Debt Servicing
- Collection
- Fintech
- Payments
- Webhook
- Financial-Services
- Dunning
---
