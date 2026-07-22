---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: supio.com
  spf: true
hosts:
- cert_expires: Oct 16 01:01:03 2026 GMT
  host: supio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Supio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Supio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Supio
provider_slug: supio
slug: supio-domain-security
source_filename: supio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: supio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 01:01:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: supio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supio/refs/heads/main/security/supio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal
- Legal Tech
- Artificial Intelligence
- Agentic AI
- Personal Injury
- Document Automation
- Case Management
---
