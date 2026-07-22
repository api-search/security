---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: smarterdx.com
  spf: true
hosts:
- cert_expires: Sep  6 09:16:07 2026 GMT
  host: smarterdx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smarterdx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmarterDx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SmarterDx
provider_slug: smarterdx
slug: smarterdx-domain-security
source_filename: smarterdx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smarterdx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 09:16:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: smarterdx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smarterdx/refs/heads/main/security/smarterdx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Clinical AI
- Revenue Cycle Management
- Health Systems
- Clinical Documentation
- HIPAA
- Artificial Intelligence
---
