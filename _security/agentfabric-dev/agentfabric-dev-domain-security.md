---
api_specs:
- filename: agentfabric-dev-openapi-generated.yml
  format: yaml
  label: agentfabric-dev API
  slug: agentfabric-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentfabric-dev/openapi/_ae-authored/agentfabric-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agentfabric.dev
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: agentfabric.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentfabric Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for agentfabric-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: agentfabric-dev
provider_slug: agentfabric-dev
slug: agentfabric-dev-domain-security
source_filename: agentfabric-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentfabric.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: agentfabric.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agentfabric-dev/security/agentfabric-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- HumanReview
- MCP
- REST
- Automation
---
