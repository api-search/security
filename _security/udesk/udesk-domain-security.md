---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: udesk.cn
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.udesk.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: demo.udesk.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: km.udesk.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Udesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Udesk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Udesk
provider_slug: udesk
slug: udesk-domain-security
source_filename: udesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.udesk.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\n- host: demo.udesk.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\n- host: km.udesk.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: udesk.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/udesk/refs/heads/main/security/udesk-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Enterprise
- Customer Service
- Call Center
- Ticketing
- Chatbots
- CRM
- Knowledge Management
- SaaS
- China
---
