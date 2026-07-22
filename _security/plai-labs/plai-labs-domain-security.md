---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: salt.ai
  spf: true
hosts:
- cert_expires: Sep  5 03:50:18 2026 GMT
  host: docs.salt.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 19:25:01 2026 GMT
  host: salt-api-dev.salt.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plai Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plai Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plai Labs
provider_slug: plai-labs
slug: plai-labs-domain-security
source_filename: plai-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.salt.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 03:50:18 2026 GMT\n  hsts: false\n- host: salt-api-dev.salt.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:25:01 2026 GMT\n  hsts: false\ndomains:\n- domain: salt.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plai-labs/refs/heads/main/security/plai-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- AI Workflows
- Agents
- LLM
- Enterprise
- Regulated Industries
- Life Sciences
- Workflow Automation
- No-Code
---
