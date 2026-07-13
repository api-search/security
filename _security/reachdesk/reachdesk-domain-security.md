---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reachdesk.com
  spf: true
hosts:
- cert_expires: Aug 29 12:18:28 2026 GMT
  host: www.reachdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:41:35 2026 GMT
  host: support.reachdesk.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: app.reachdesk.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reachdesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reachdesk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reachdesk
provider_slug: reachdesk
slug: reachdesk-domain-security
source_filename: reachdesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reachdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 12:18:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.reachdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:41:35 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: app.reachdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: reachdesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reachdesk/refs/heads/main/security/reachdesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Corporate Gifting
- Direct Mail
- Swag
- B2B
- Sales Enablement
- Customer Success
- Marketing Automation
- Gifting Platform
- Rewards
---
