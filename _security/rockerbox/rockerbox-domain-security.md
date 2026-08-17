---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rockerbox.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: getrockerbox.com
  spf: true
hosts:
- cert_expires: Sep 28 17:02:06 2026 GMT
  host: www.rockerbox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 12:46:16 2026 GMT
  host: help.rockerbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 22:05:55 2026 GMT
  host: webhooks.getrockerbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rockerbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rockerbox, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rockerbox
provider_slug: rockerbox
slug: rockerbox-domain-security
source_filename: rockerbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rockerbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:02:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.rockerbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 12:46:16 2026 GMT\n  hsts: false\n- host: webhooks.getrockerbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 22:05:55 2026 GMT\n  hsts: false\ndomains:\n- domain: rockerbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getrockerbox.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockerbox/refs/heads/main/security/rockerbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Marketing Attribution
- Multi-Touch Attribution
- Marketing Mix Modeling
- Incrementality Testing
- Media Spend
- Customer Journeys
- Marketing Analytics
- Data Warehousing
- Conversion Tracking
- Webhooks
---
