---
api_specs:
- filename: policycheck-tools-openapi.yml
  format: yaml
  label: PolicyCheck API
  slug: policycheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/policycheck-tools/refs/heads/main/openapi/policycheck-tools-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: policycheck.tools
  spf: true
hosts:
- cert_expires: Nov 20 02:50:27 2026 GMT
  host: policycheck.tools
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Policycheck Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PolicyCheck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PolicyCheck
provider_slug: policycheck-tools
slug: policycheck-tools-domain-security
source_filename: policycheck-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: policycheck.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:50:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: policycheck.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/policycheck-tools/refs/heads/main/security/policycheck-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Policy Analysis
- Consumer Protection
- E-Commerce
- Agentic Commerce
- Risk Assessment
- AI Agents
- A2A
- MCP
- x402
- Legal
- Returns
---
