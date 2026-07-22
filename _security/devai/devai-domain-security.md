---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dev-ai.com
  spf: true
hosts:
- cert_expires: Oct  8 02:12:08 2026 GMT
  host: dev-ai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Devai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DevAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DevAI
provider_slug: devai
slug: devai-domain-security
source_filename: devai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 02:12:08 2026 GMT\n  hsts: false\ndomains:\n- domain: dev-ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devai/refs/heads/main/security/devai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Developer Tools
- IT Operations
- Artificial Intelligence
- AI Agents
- Enterprise IT
- Network Intelligence
- Incident Response
- Infrastructure Management
---
