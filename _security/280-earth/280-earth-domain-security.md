---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 280.earth
  spf: true
hosts:
- cert_expires: Sep 14 09:32:58 2026 GMT
  host: 280.earth
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 280 Earth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 280 Earth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 280 Earth
provider_slug: 280-earth
slug: 280-earth-domain-security
source_filename: 280-earth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 280.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:32:58 2026 GMT\n  hsts: false\ndomains:\n- domain: 280.earth\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/280-earth/refs/heads/main/security/280-earth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Climate
- Carbon Removal
- Direct Air Capture
- Carbon Capture
- Sustainability
- Energy
- Climate Tech
---
