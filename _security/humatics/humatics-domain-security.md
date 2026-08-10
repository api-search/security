---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: humatics.com
  spf: true
hosts:
- cert_expires: Sep 29 11:43:23 2026 GMT
  host: humatics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humatics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humatics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Humatics
provider_slug: humatics
slug: humatics-domain-security
source_filename: humatics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humatics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:43:23 2026 GMT\n  hsts: null\ndomains:\n- domain: humatics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humatics/refs/heads/main/security/humatics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Positioning
- Microlocation
- Ultra-Wideband
- Sensors
- Navigation
- Robotics
- Industrial Automation
- Rail
- Transit
- Manufacturing
- Hardware
---
