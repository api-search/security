---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: getsatisfaction.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: getsatisfaction.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Get Satisfaction Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Get Satisfaction, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Get Satisfaction
provider_slug: get-satisfaction
slug: get-satisfaction-domain-security
source_filename: get-satisfaction-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getsatisfaction.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getsatisfaction.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/get-satisfaction/refs/heads/main/security/get-satisfaction-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
- Customer Community
- Customer Engagement
- Customer Support
- Community Platform
- Social Media
- SaaS
- Acquired
---
