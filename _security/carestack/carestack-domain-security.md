---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carestack.com
  spf: true
hosts:
- cert_expires: Sep 15 03:35:35 2026 GMT
  host: www.carestack.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carestack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CareStack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CareStack
provider_slug: carestack
slug: carestack-domain-security
source_filename: carestack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carestack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:35:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: carestack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carestack/refs/heads/main/security/carestack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Dental
- Practice Management
- Electronic Health Records
- Revenue Cycle Management
- Patient Engagement
- Payments
- SaaS
---
