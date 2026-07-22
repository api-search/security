---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: schematiclabs.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: soundtracking.com
  spf: false
hosts:
- cert_expires: '2027-01-29'
  content: domain-parking lander (JS redirect to /lander)
  host: schematiclabs.com
  hsts: false
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: '2026-09-29'
  host: soundtracking.com
  hsts: false
  http_status: 301
  https: true
  redirects_to: https://www.napster.com/
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schematic Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schematic Labs, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Schematic Labs
provider_slug: schematic-labs
slug: schematic-labs-domain-security
source_filename: schematic-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: dig + TLS/HTTP HEAD probes of the company's historical domains\nnote: >-\n  Schematic Labs is a defunct company (acquired by Rhapsody in August 2014).\n  schematiclabs.com now serves a domain-parking lander and soundtracking.com\n  301-redirects to www.napster.com (Rhapsody's successor brand), so this\n  records the posture of the historical domain trail, not an operating\n  provider surface.\nhosts:\n  - host: schematiclabs.com\n    https: true\n    http_status: 200\n    tls_version: TLSv1.3\n    cert_expires: '2027-01-29'\n    hsts: false\n    content: domain-parking lander (JS redirect to /lander)\n  - host: soundtracking.com\n    https: true\n    http_status: 301\n    redirects_to: https://www.napster.com/\n    server: cloudflare\n    tls_version: TLSv1.3\n    cert_expires: '2026-09-29'\n    hsts: false\ndomains:\n  - domain: schematiclabs.com\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n  - domain:\
  \ soundtracking.com\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schematic-labs/refs/heads/main/security/schematic-labs-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Music
- Social
- Mobile
- Acquired
- Defunct
---
