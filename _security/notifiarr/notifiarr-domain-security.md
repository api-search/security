---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: notifiarr.com
  spf: true
hosts:
- cert_expires: Jan  8 14:00:47 2027 GMT
  host: notifiarr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Notifiarr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Notifiarr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Notifiarr
provider_slug: notifiarr
slug: notifiarr-domain-security
source_filename: notifiarr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: notifiarr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 14:00:47 2027 GMT\n  hsts: false\ndomains:\n- domain: notifiarr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/notifiarr/security/notifiarr-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Notification
- Monitoring
- Integration
- OpenSource
---
