---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vortexify.ai
  spf: true
hosts:
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: www.vortexify.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Praxis Ai 2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Praxis AI (Vortexify), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Praxis AI (Vortexify)
provider_slug: praxis-ai-2
slug: praxis-ai-2-domain-security
source_filename: praxis-ai-2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vortexify.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: vortexify.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/praxis-ai-2/refs/heads/main/security/praxis-ai-2-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- No-Code
- Data Integration
- Application Development
- AI Agents
- Automation
- Manufacturing
---
