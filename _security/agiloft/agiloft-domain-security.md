---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agiloft.com
  spf: true
hosts:
- cert_expires: Dec  9 14:58:39 2026 GMT
  host: www.agiloft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 00:17:09 2026 GMT
  host: help.agiloft.com
  hsts: true
  hsts_max_age: 34560000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Agiloft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agiloft, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agiloft
provider_slug: agiloft
slug: agiloft-domain-security
source_filename: agiloft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agiloft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 14:58:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.agiloft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 00:17:09 2026 GMT\n  hsts: true\n  hsts_max_age: 34560000\ndomains:\n- domain: agiloft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agiloft/refs/heads/main/security/agiloft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Contract Lifecycle Management
- Contract Management
- Legal
- Procurement
- Enterprise Software
- No-Code
- Workflow-Automation
- Document Automation
- Webhook
- SCIM
- Company
---
