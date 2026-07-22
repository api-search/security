---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pointee.ai
  spf: false
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.pointee.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pointee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pointee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Pointee
provider_slug: pointee
slug: pointee-domain-security
source_filename: pointee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pointee.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: pointee.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pointee/refs/heads/main/security/pointee-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Automation
- Business Process Automation
- RPA
- Agentic Automation
- AI Agents
- Workflow Automation
- Process Discovery
---
