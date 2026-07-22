---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wanderu.com
  spf: true
hosts:
- cert_expires: Sep 18 20:32:04 2026 GMT
  host: wanderu.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wanderu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wanderu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wanderu
provider_slug: wanderu
slug: wanderu-domain-security
source_filename: wanderu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wanderu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:32:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: wanderu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wanderu/refs/heads/main/security/wanderu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Transportation
- Bus
- Train
- Booking
- Metasearch
- Ticketing
---
