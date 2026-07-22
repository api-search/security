---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dialoguslabs.com
  spf: false
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: www.dialoguslabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dialogus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dialogus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dialogus
provider_slug: dialogus
slug: dialogus-domain-security
source_filename: dialogus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dialoguslabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dialoguslabs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dialogus/refs/heads/main/security/dialogus-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Voice Agents
- AI Agents
- Conversational AI
- Customer Support
- Contact Center
- Collections
- Compliance
---
