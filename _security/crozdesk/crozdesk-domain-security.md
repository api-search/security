---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crozdesk.com
  spf: true
hosts:
- cert_expires: Sep 26 22:01:11 2026 GMT
  host: crozdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 10:17:28 2026 GMT
  host: vendor.crozdesk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crozdesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crozdesk, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crozdesk
provider_slug: crozdesk
slug: crozdesk-domain-security
source_filename: crozdesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crozdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:01:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vendor.crozdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 10:17:28 2026 GMT\n  hsts: false\ndomains:\n- domain: crozdesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crozdesk/refs/heads/main/security/crozdesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- SaaS
- Software Discovery
- Reviews
- Vendor Marketplace
---
