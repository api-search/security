---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tae.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: tae.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tae Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TAE Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TAE Technologies
provider_slug: tae-technologies
slug: tae-technologies-domain-security
source_filename: tae-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tae.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tae.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tae-technologies/refs/heads/main/security/tae-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fusion Energy
- Aneutronic Fusion
- Hydrogen Boron
- p-B11
- Field-Reversed Configuration
- Plasma Physics
- Clean Energy
- Baseload Power
- BNCT
- Cancer Therapy
- Power Electronics
- E-Mobility
- Battery Management
- Deep Tech
- Hardware
---
