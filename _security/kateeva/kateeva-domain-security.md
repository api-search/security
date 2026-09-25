---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kateeva.com
  spf: true
hosts:
- cert_expires: Oct 20 10:49:10 2026 GMT
  host: kateeva.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kateeva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kateeva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kateeva
provider_slug: kateeva
slug: kateeva-domain-security
source_filename: kateeva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kateeva.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 20 10:49:10 2026 GMT\n  hsts: false\ndomains:\n- domain: kateeva.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/security/kateeva-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Display Manufacturing
- OLED
- Semiconductor Equipment
- Capital Equipment
- Inkjet Printing
- Thin Film Encapsulation
- Advanced Manufacturing
- Materials Deposition
- Consumer Electronics
- Hardware
---
