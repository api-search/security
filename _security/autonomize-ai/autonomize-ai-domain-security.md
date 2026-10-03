---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: autonomize.ai
  spf: true
hosts:
- cert_expires: Dec 14 17:07:37 2026 GMT
  host: autonomize.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Autonomize Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autonomize AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Autonomize AI
provider_slug: autonomize-ai
slug: autonomize-ai-domain-security
source_filename: autonomize-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autonomize.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 17:07:37 2026 GMT\n  hsts: false\ndomains:\n- domain: autonomize.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autonomize-ai/refs/heads/main/security/autonomize-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Healthcare
- Automation
- Autonomy
---
