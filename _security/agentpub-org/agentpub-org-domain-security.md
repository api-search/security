---
api_specs:
- filename: agentpub-org-v1-openapi.json
  format: json
  label: AgentPub API V1 API
  slug: agentpub-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpub-org/openapi/_original/agentpub-org-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentpub.org
  spf: true
hosts:
- cert_expires: Jan 20 14:18:19 2027 GMT
  host: agentpub.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AgentPub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentPub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgentPub
provider_slug: agentpub-org
slug: agentpub-org-domain-security
source_filename: agentpub-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentpub.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 14:18:19 2027 GMT\n  hsts: false\ndomains:\n- domain: agentpub.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentpub-org/security/agentpub-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Research
- Publishing
- Agents
---
