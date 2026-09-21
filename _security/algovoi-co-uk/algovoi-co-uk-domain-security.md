---
api_specs:
- filename: algovoi-co-uk-pay-openapi.yml
  format: yaml
  label: AlgoVoi Pay (Payable Core) API
  slug: algovoi-pay-payable-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-pay-openapi.yml
- filename: algovoi-co-uk-gateway-openapi.yml
  format: yaml
  label: AlgoVoi Gateway API
  slug: algovoi-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-gateway-openapi.yml
- filename: algovoi-co-uk-clinic-openapi.yml
  format: yaml
  label: AlgoVoi RFC 9421 Clinic (Verifiable-Comms Agent) API
  slug: algovoi-rfc9421-clinic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-clinic-openapi.yml
- filename: algovoi-co-uk-agent-trust-bench-openapi.yml
  format: yaml
  label: AlgoVoi Agent Trust Bench API
  slug: algovoi-agent-trust-bench-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-agent-trust-bench-openapi.yml
- filename: algovoi-co-uk-audit-verifier-openapi.yml
  format: yaml
  label: AlgoVoi Audit Verifier API
  slug: algovoi-audit-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-audit-verifier-openapi.yml
- filename: algovoi-co-uk-gateway-openapi.yml
  format: yaml
  label: AlgoVoi MCP Server
  slug: algovoi-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-gateway-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: algovoi.co.uk
  spf: true
hosts:
- cert_expires: Nov  3 19:45:42 2026 GMT
  host: algovoi.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 19:45:42 2026 GMT
  host: docs.algovoi.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 19:45:42 2026 GMT
  host: pay.algovoi.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Algovoi Co Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlgoVoi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AlgoVoi
provider_slug: algovoi-co-uk
slug: algovoi-co-uk-domain-security
source_filename: algovoi-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: algovoi.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 19:45:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.algovoi.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 19:45:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pay.algovoi.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 19:45:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: algovoi.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/security/algovoi-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Agentic Commerce
- x402
- A2A
- MCP
- Stablecoins
- Cryptocurrency
- Blockchain
- Compliance
- Digital Signature
- Post-Quantum Cryptography
- Verification
- Fintech
- agent-native
- Algorand
- United Kingdom
---
