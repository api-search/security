---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: markt-pilot.com
  spf: true
hosts:
- cert_expires: Oct 10 11:13:21 2026 GMT
  host: www.markt-pilot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Markt Pilot Aka Mp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Markt Pilot (aka MP), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Markt Pilot (aka MP)
provider_slug: markt-pilot-aka-mp
slug: markt-pilot-aka-mp-domain-security
source_filename: markt-pilot-aka-mp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.markt-pilot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 11:13:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: markt-pilot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/markt-pilot-aka-mp/refs/heads/main/security/markt-pilot-aka-mp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pricing
- Pricing Intelligence
- Spare Parts
- Manufacturing
- Industrial Equipment
- Market Intelligence
- Aftermarket
---
