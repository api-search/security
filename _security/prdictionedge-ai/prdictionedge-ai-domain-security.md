---
api_specs:
- filename: prdictionedge-ai-openapi.yml
  format: yaml
  label: AUX Evidence and Certification API
  slug: aux-evidence-and-certification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prdictionedge-ai/refs/heads/main/openapi/prdictionedge-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prdictionedge.ai
  spf: true
hosts:
- cert_expires: Oct 24 02:19:01 2026 GMT
  host: prdictionedge.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 14:30:23 2026 GMT
  host: aux.prdictionedge.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 07:56:03 2026 GMT
  host: api.aux.prdictionedge.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Prdictionedge Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AUX by PrdictionEdge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AUX by PrdictionEdge
provider_slug: prdictionedge-ai
slug: prdictionedge-ai-domain-security
source_filename: prdictionedge-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prdictionedge.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 02:19:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: aux.prdictionedge.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 14:30:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.aux.prdictionedge.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 07:56:03 2026 GMT\n  hsts: null\ndomains:\n- domain: prdictionedge.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prdictionedge-ai/refs/heads/main/security/prdictionedge-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Counterparty Verification
- Sanctions Screening
- Legal Entity Identifier
- KYB
- Agent Infrastructure
- Trust and Safety
- Signed Receipts
- Agentic Payments
- A2A
- Agent-Native
---
