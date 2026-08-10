---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ursamajor.com
  spf: true
hosts:
- cert_expires: Oct  3 02:39:36 2026 GMT
  host: ursamajor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ursa Major Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ursa Major Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ursa Major Technologies
provider_slug: ursa-major-technologies
slug: ursa-major-technologies-domain-security
source_filename: ursa-major-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ursamajor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:39:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ursamajor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ursa-major-technologies/refs/heads/main/security/ursa-major-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Aerospace
- Defense
- Propulsion
- Rocket Engines
- Solid Rocket Motors
- Hypersonics
- Space
- Satellites
- Missile Defense
- Additive Manufacturing
- Manufacturing
- National Security
- Colorado
---
