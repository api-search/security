---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gm.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: developer.gm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: General Motors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for General Motors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: General Motors
provider_slug: general-motors
slug: general-motors-domain-security
source_filename: general-motors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.gm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: gm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/general-motors/refs/heads/main/security/general-motors-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automobiles
- Cars
- Vehicles
- Connected Vehicles
- Telematics
- Fortune 100
---
