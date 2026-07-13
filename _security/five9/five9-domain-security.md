---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: five9.com
  spf: true
hosts:
- cert_expires: Jul 23 20:41:52 2026 GMT
  host: www.five9.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: app.five9.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: documentation.five9.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Five9 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Five9, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Five9
provider_slug: five9
slug: five9-domain-security
source_filename: five9-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.five9.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 23 20:41:52 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: app.five9.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.five9.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: five9.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/five9/refs/heads/main/security/five9-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Contact Center
- CCaaS
- Cloud Telephony
- Customer Engagement
- Omnichannel
- Workforce Optimization
- Virtual Agents
---
