---
api_specs:
- filename: knostic-agentmesh-openapi.yml
  format: yaml
  label: Knostic AgentMesh API
  slug: agentmesh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knostic/refs/heads/main/openapi/knostic-agentmesh-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: knostic.ai
  spf: true
hosts:
- cert_expires: Oct 11 13:47:20 2026 GMT
  host: knostic.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 19:31:56 2026 GMT
  host: agentmesh.knostic.ai
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knostic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knostic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Knostic
provider_slug: knostic
slug: knostic-domain-security
source_filename: knostic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knostic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 13:47:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: agentmesh.knostic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:31:56 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: knostic.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knostic/refs/heads/main/security/knostic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Artificial Intelligence
- AI Agents
- Agent Security
- Supply Chain Security
- Model Context Protocol
- Threat Intelligence
- Developer Tools
- Shadow AI
---
