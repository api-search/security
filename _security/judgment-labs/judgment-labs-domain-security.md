---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: judgmentlabs.ai
  spf: true
hosts:
- cert_expires: Sep 21 13:43:45 2026 GMT
  host: www.judgmentlabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 19:41:23 2026 GMT
  host: docs.judgmentlabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: api.judgmentlabs.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Judgment Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Judgment Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Judgment Labs
provider_slug: judgment-labs
slug: judgment-labs-domain-security
source_filename: judgment-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.judgmentlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:43:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.judgmentlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 19:41:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.judgmentlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: judgmentlabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/judgment-labs/refs/heads/main/security/judgment-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agents
- Artificial Intelligence
- Agent Evaluation
- Observability
- Tracing
- Monitoring
- LLM
- Developer Tools
- MCP
---
