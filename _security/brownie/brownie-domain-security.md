---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: incidentfox.ai
  spf: false
hosts:
- cert_expires: Sep  4 17:08:58 2026 GMT
  host: docs.incidentfox.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.incidentfox.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Brownie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IncidentFox (Brownie), probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: IncidentFox (Brownie)
provider_slug: brownie
slug: brownie-domain-security
source_filename: brownie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.incidentfox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 17:08:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.incidentfox.ai\n  https: false\ndomains:\n- domain: incidentfox.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brownie/refs/heads/main/security/brownie-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Incident Response
- SRE
- AIOps
- Observability
- DevOps
- Artificial Intelligence
- Developer Tools
- Automation
- Open Source
---
