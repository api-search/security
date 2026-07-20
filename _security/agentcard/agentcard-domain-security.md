---
api_specs:
- filename: agentcard-openapi-original.json
  format: json
  label: Agentcard v2 API
  slug: agentcard-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentcard/refs/heads/main/openapi/agentcard-openapi-original.json
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentcard/refs/heads/main/security/agentcard-domain-security.yml
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
- Wallet
- Visa
---
