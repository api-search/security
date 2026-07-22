---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beatdapp.com
  spf: true
hosts:
- cert_expires: Aug 30 21:17:55 2026 GMT
  host: beatdapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beatdapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beatdapp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Beatdapp
provider_slug: beatdapp
slug: beatdapp-domain-security
source_filename: beatdapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beatdapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 21:17:55 2026 GMT\n  hsts: false\ndomains:\n- domain: beatdapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beatdapp/refs/heads/main/security/beatdapp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Trust and Safety
- Fraud Detection
- Music Streaming
- Anomaly Detection
- Content Integrity
- AI Detection
- Account Security
---
