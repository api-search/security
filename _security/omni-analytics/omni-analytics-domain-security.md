---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: exploreomni.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: omni.co
  spf: true
hosts:
- cert_expires: Oct  3 17:43:58 2026 GMT
  host: exploreomni.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 12 23:50:15 2026 GMT
  host: docs.omni.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: omniapp.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Omni Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omni Analytics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Omni Analytics
provider_slug: omni-analytics
slug: omni-analytics-domain-security
source_filename: omni-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exploreomni.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 17:43:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.omni.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 12 23:50:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: omniapp.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: exploreomni.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: omni.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omni-analytics/refs/heads/main/security/omni-analytics-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Enterprise
- Analytics
- Business Intelligence
- Embedded Analytics
- Semantic Layer
- Artificial Intelligence
- Data
- MCP
---
