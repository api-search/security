---
api_specs:
- filename: agentdrive-sh-openapi-generated.yml
  format: yaml
  label: AgentDrive API
  slug: agentdrive-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdrive-sh/openapi/_ae-authored/agentdrive-sh-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agentdrive.sh
  spf: true
hosts:
- cert_expires: Jan 19 20:49:15 2027 GMT
  host: agentdrive.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AgentDrive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentDrive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AgentDrive
provider_slug: agentdrive-sh
slug: agentdrive-sh-domain-security
source_filename: agentdrive-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentdrive.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 20:49:15 2027 GMT\n  hsts: false\ndomains:\n- domain: agentdrive.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/agentdrive-sh/security/agentdrive-sh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AgentDrive
- Artificial Intelligence
- Multi-Agent
- Workspace
- Memory
- MCP
---
