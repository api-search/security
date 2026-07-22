---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lightshiprv.com
  spf: true
hosts:
- cert_expires: Sep 18 16:04:47 2026 GMT
  host: lightshiprv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightship Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightship, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lightship
provider_slug: lightship
slug: lightship-domain-security
source_filename: lightship-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightshiprv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 16:04:47 2026 GMT\n  hsts: false\ndomains:\n- domain: lightshiprv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightship/refs/heads/main/security/lightship-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Electric Vehicles
- Automotive
- Manufacturing
- Clean Energy
- Travel
- Outdoor Recreation
- Consumer Hardware
- Sustainability
---
