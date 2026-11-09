---
api_specs:
- filename: agentcat-com-openapi-generated.yml
  format: yaml
  label: AgentCat API
  slug: agentcat-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcat-com/openapi/_ae-authored/agentcat-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentcat.com
  spf: true
hosts:
- cert_expires: Dec  1 15:31:21 2026 GMT
  host: agentcat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentcat Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentCat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgentCat
provider_slug: agentcat-com
slug: agentcat-com-domain-security
source_filename: agentcat-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentcat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 15:31:21 2026 GMT\n  hsts: false\ndomains:\n- domain: agentcat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentcat-com/security/agentcat-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Analytics
- Observability
- Agent Experience
- Company
---
