---
api_specs:
- filename: swopme-co-control-api-openapi.yml
  format: yaml
  label: Swop Control API
  slug: swopme-co-control-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-control-api-openapi.yml
- filename: swopme-co-oidc-api-openapi.yml
  format: yaml
  label: Swop Oidc API
  slug: swopme-co-oidc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-oidc-api-openapi.yml
- filename: swopme-co-runtime-accounts-api-openapi.yml
  format: yaml
  label: Swop Runtime Accounts API
  slug: swopme-co-runtime-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-runtime-accounts-api-openapi.yml
- filename: swopme-co-runtime-auth-api-openapi.yml
  format: yaml
  label: Swop Runtime Auth API
  slug: swopme-co-runtime-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-runtime-auth-api-openapi.yml
- filename: swopme-co-runtime-intents-api-openapi.yml
  format: yaml
  label: Swop Runtime Intents API
  slug: swopme-co-runtime-intents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-runtime-intents-api-openapi.yml
- filename: swopme-co-runtime-session-grants-api-openapi.yml
  format: yaml
  label: Swop Runtime Session Grants API
  slug: swopme-co-runtime-session-grants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-runtime-session-grants-api-openapi.yml
- filename: swopme-co-runtime-sponsorship-api-openapi.yml
  format: yaml
  label: Swop Runtime Sponsorship API
  slug: swopme-co-runtime-sponsorship-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-runtime-sponsorship-api-openapi.yml
- filename: swopme-co-server-users-api-openapi.yml
  format: yaml
  label: Swop Server Users API
  slug: swopme-co-server-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-server-users-api-openapi.yml
- filename: swopme-co-server-wallets-api-openapi.yml
  format: yaml
  label: Swop Server Wallets API
  slug: swopme-co-server-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-server-wallets-api-openapi.yml
- filename: swopme-co-server-webhooks-api-openapi.yml
  format: yaml
  label: Swop Server Webhooks API
  slug: swopme-co-server-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-server-webhooks-api-openapi.yml
- filename: swopme-co-system-api-openapi.yml
  format: yaml
  label: Swop System API
  slug: swopme-co-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: swopme.co
  spf: true
hosts:
- cert_expires: Jan 31 17:55:19 2027 GMT
  host: swopme.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Swop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Swop
provider_slug: swopme-co
slug: swopme-co-domain-security
source_filename: swopme-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swopme.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 17:55:19 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: swopme.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/swopme-co/security/swopme-co-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- FinTech
- Identity
- Payments
- AI
- Wallet
---
