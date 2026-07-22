---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ritasice.com
  spf: true
hosts:
- cert_expires: Oct 14 14:23:54 2026 GMT
  host: www.ritasice.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ritas Italian Ice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rita''s Italian Ice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rita's Italian Ice
provider_slug: ritas-italian-ice
slug: ritas-italian-ice-domain-security
source_filename: ritas-italian-ice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ritasice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 14:23:54 2026 GMT\n  hsts: false\ndomains:\n- domain: ritasice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ritas-italian-ice/refs/heads/main/security/ritas-italian-ice-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Restaurants
- Food and Beverage
- Frozen Desserts
- Franchise
- Quick Service Restaurant
---
