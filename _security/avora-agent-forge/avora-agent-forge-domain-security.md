---
api_specs:
- filename: avora-agent-forge-agent-api-openapi.yml
  format: yaml
  label: AVORA Agent Forge Agent API
  slug: avora-agent-forge-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avora-agent-forge/refs/heads/main/openapi/avora-agent-forge-agent-api-openapi.yml
- filename: avora-agent-forge-public-evidence-api-openapi.yml
  format: yaml
  label: AVORA Agent Forge Public Evidence API
  slug: avora-agent-forge-public-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avora-agent-forge/refs/heads/main/openapi/avora-agent-forge-public-evidence-api-openapi.yml
description: ''
domains:
- caa:
  - 128 iodef "mailto:security@netlify.com"
  - 128 issue "digicert.com;account=2d83e9ac9b6776c3f215150f6ebceea8cefe3bc2e1fb5efffb1d71e200575226"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netlify.app
  owner: Netlify (hosting platform, not the API provider)
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: avora-agent-forge.netlify.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avora Agent Forge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AVORA Agent Forge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AVORA Agent Forge
provider_slug: avora-agent-forge
slug: avora-agent-forge-domain-security
source_filename: avora-agent-forge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avora-agent-forge.netlify.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomain_ownership_caveat: >-\n  AVORA does not operate a branded apex domain - the service is hosted at\n  avora-agent-forge.netlify.app, so the registrable domain below is netlify.app, the hosting\n  platform's. The DNSSEC, CAA, SPF, and DMARC records recorded under `domains` are\n  Netlify's posture, NOT AVORA's, and must not be read as this provider's own domain\n  security. Only the `hosts` block (TLS and HSTS on the serving host) reflects a\n  configuration AVORA is responsible for, and even HSTS is a platform default. AVORA\n  controls no DNS zone of its own and therefore publishes no CAA, SPF, or DMARC.\ndomains:\n- domain: netlify.app\n  owner: Netlify (hosting platform, not the API provider)\n  dnssec:\
  \ false\n  caa:\n  - 128 iodef \"mailto:security@netlify.com\"\n  - 128 issue \"digicert.com;account=2d83e9ac9b6776c3f215150f6ebceea8cefe3bc2e1fb5efffb1d71e200575226\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avora-agent-forge/refs/heads/main/security/avora-agent-forge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Crypto
- Solana
- Token Risk
- Due Diligence
- On-chain Evidence
- Fraud Intelligence
- AI Agents
- MCP
- A2A
- Signed Receipts
- Provenance
- Non-custodial Payments
- USDC
- Solana Pay
- Public-sector AI Interoperability
---
