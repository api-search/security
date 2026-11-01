---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: canopyaerospace.com
  spf: true
hosts:
- cert_expires: Jan 21 16:12:54 2027 GMT
  host: canopyaerospace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Canopyaerospace Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canopy Aerospace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Canopy Aerospace
provider_slug: canopyaerospace-com
slug: canopyaerospace-com-domain-security
source_filename: canopyaerospace-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canopyaerospace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 16:12:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: canopyaerospace.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/canopyaerospace-com/security/canopyaerospace-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Aerospace
- Defense
- Manufacturing
- Innovation
---
