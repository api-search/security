---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: filingdesk.com
  spf: true
hosts:
- cert_expires: Dec 18 04:13:46 2026 GMT
  host: filingdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Filingdesk Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FilingDesk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FilingDesk
provider_slug: filingdesk-com
slug: filingdesk-com-domain-security
source_filename: filingdesk-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: filingdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 04:13:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: filingdesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/filingdesk-com/security/filingdesk-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- LLC Formation
- Business Formation
- Company Registration
- EIN
- Operating Agreement
- Registered Agent
- Compliance
- AI Agents
- MCP
- SMB
---
