---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: popmenu.com
  spf: true
hosts:
- cert_expires: Sep 29 23:35:22 2026 GMT
  host: get.popmenu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Popmenu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Popmenu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Popmenu
provider_slug: popmenu
slug: popmenu-domain-security
source_filename: popmenu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: get.popmenu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:35:22 2026 GMT\n  hsts: null\ndomains:\n- domain: popmenu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/popmenu/refs/heads/main/security/popmenu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Restaurant
- Menus
- Online Ordering
- Websites
- Marketing
- Integration
- Hospitality
- GraphQL
- Point-of-Sale
- Reservations
- Loyalty
- AI Marketing
---
