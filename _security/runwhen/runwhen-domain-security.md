---
api_specs:
- filename: runwhen-papi-openapi-original.json
  format: json
  label: RunWhen Platform API (PAPI)
  slug: runwhen-platform-api-papi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwhen/refs/heads/main/openapi/runwhen-papi-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: runwhen.com
  spf: true
hosts:
- cert_expires: Oct  3 13:32:54 2026 GMT
  host: runwhen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runwhen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RunWhen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: RunWhen
provider_slug: runwhen
slug: runwhen-domain-security
source_filename: runwhen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runwhen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:32:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: runwhen.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runwhen/refs/heads/main/security/runwhen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AIOps
- SRE
- DevOps
- Observability
- Incident Response
- AI Agents
- Kubernetes
- Automation
- MCP
---
