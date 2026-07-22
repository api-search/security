---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: basata.ai
  spf: true
hosts:
- cert_expires: Sep 20 21:45:11 2026 GMT
  host: www.basata.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Basata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Basata
provider_slug: basata
slug: basata-domain-security
source_filename: basata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.basata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 21:45:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: basata.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basata/refs/heads/main/security/basata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Artificial Intelligence
- AI Agents
- Health IT
- Medical Practice Administration
- Voice AI
- Automation
- HIPAA
---
