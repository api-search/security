---
api_specs:
- filename: privatedao-org-agent-exchange-openapi.yml
  format: yaml
  label: PrivateDAO Agent Exchange API
  slug: agent-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-agent-exchange-openapi.yml
- filename: privatedao-org-blind-policy-openapi.yml
  format: yaml
  label: PrivateDAO Blind Policy Verification API
  slug: blind-policy-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/openapi/privatedao-org-blind-policy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: privatedao.org
  spf: true
hosts:
- cert_expires: Nov  7 00:09:26 2026 GMT
  host: privatedao.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: agents.privatedao.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 15:22:06 2026 GMT
  host: api.privatedao.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Privatedao Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PrivateDAO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PrivateDAO
provider_slug: privatedao-org
slug: privatedao-org-domain-security
source_filename: privatedao-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: privatedao.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 00:09:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: agents.privatedao.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: null\n- host: api.privatedao.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 15:22:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: privatedao.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/privatedao-org/refs/heads/main/security/privatedao-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Agents
- A2A
- MCP
- Verification
- Zero-Knowledge Proofs
- Solana
- Blockchain
- Payments
- Marketplace
- Privacy
- Governance
- Treasury
---
