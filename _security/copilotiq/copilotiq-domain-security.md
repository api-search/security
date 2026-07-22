---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: copilotiq.com
  spf: true
hosts:
- cert_expires: Oct  5 08:33:28 2026 GMT
  host: copilotiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Copilotiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CopilotIQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: CopilotIQ
provider_slug: copilotiq
slug: copilotiq-domain-security
source_filename: copilotiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: copilotiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 08:33:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: copilotiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copilotiq/refs/heads/main/security/copilotiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Remote Patient Monitoring
- Telehealth
- Chronic Disease Management
- Digital Health
- Medicare
---
