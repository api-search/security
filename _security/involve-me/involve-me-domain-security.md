---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: involve.me
  spf: true
hosts:
- cert_expires: Oct 11 09:02:05 2026 GMT
  host: www.involve.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 22:24:52 2026 GMT
  host: www-cdn.involve.me
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Involve Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for involve.me, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: involve.me
provider_slug: involve-me
slug: involve-me-domain-security
source_filename: involve-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.involve.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 09:02:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www-cdn.involve.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:24:52 2026 GMT\n  hsts: false\ndomains:\n- domain: involve.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/involve-me/refs/heads/main/security/involve-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Lead Generation
- Forms
- Surveys
- Quizzes
- No-Code
- Email Marketing
- CRM
- Webhook
- MCP
- Austria
---
