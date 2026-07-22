---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: woowup.com
  spf: true
hosts:
- cert_expires: Sep 19 23:15:31 2026 GMT
  host: www.woowup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 00:50:23 2026 GMT
  host: docs.woowup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: api.woowup.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Woowup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WoowUp, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WoowUp
provider_slug: woowup
slug: woowup-domain-security
source_filename: woowup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.woowup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:15:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.woowup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:50:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.woowup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: woowup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woowup/refs/heads/main/security/woowup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- Loyalty
- Customer Data
- Marketing Automation
- Retail
- eCommerce
- Push Notifications
---
