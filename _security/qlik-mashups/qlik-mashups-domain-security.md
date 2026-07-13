---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: qlik.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: qlik.dev
  spf: false
hosts:
- cert_expires: Sep 29 16:03:53 2026 GMT
  host: www.qlik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: help.qlik.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: qlik.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qlik Mashups Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qlik Mashups, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Qlik Mashups
provider_slug: qlik-mashups
slug: qlik-mashups-domain-security
source_filename: qlik-mashups-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qlik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:03:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.qlik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n- host: qlik.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: qlik.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: qlik.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qlik-mashups/refs/heads/main/security/qlik-mashups-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Business Intelligence
- Embedded Analytics
- Mashup
- Visualization
---
