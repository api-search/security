---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trywired.io
  spf: false
hosts:
- cert_expires: Nov 28 22:18:01 2026 GMT
  host: trywired.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trywired Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TryWired, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TryWired
provider_slug: trywired
slug: trywired-domain-security
source_filename: trywired-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trywired.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 22:18:01 2026 GMT\n  hsts: false\ndomains:\n- domain: trywired.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/trywired/security/trywired-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Integration
- HubSpot
- Telegram
- Twilio
- SMS
---
