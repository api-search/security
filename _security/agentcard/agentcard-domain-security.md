---
api_specs:
- filename: agentcard-authentication-api-openapi.yml
  format: yaml
  label: Agentcard Authentication API
  slug: agentcard-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcard/openapi/agentcard-authentication-api-openapi.yml
- filename: agentcard-connect-api-openapi.yml
  format: yaml
  label: Agentcard Connect API
  slug: agentcard-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcard/openapi/agentcard-connect-api-openapi.yml
- filename: agentcard-identity-verification-api-openapi.yml
  format: yaml
  label: Agentcard Identity verification API
  slug: agentcard-identity-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcard/openapi/agentcard-identity-verification-api-openapi.yml
- filename: agentcard-member-cards-api-openapi.yml
  format: yaml
  label: Agentcard Member cards API
  slug: agentcard-member-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcard/openapi/agentcard-member-cards-api-openapi.yml
- filename: agentcard-purchase-api-openapi.yml
  format: yaml
  label: Agentcard Purchase API
  slug: agentcard-purchase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcard/openapi/agentcard-purchase-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentcard.sh
  spf: false
hosts:
- cert_expires: Sep 24 17:23:40 2026 GMT
  host: api.agentcard.sh
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentcard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentcard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Agentcard
provider_slug: agentcard
slug: agentcard-domain-security
source_filename: agentcard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.agentcard.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:23:40 2026 GMT\n  hsts: null\ndomains:\n- domain: agentcard.sh\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentcard/security/agentcard-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Virtual Cards
- Card Issuing
- AI Agents
- Agentic Commerce
- MCP
- Fintech
- Wallets
- Visa
- A2A
---
