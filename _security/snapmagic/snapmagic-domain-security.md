---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: snapmagic.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: snapeda.com
  spf: true
hosts:
- cert_expires: Oct 14 17:07:42 2026 GMT
  host: www.snapmagic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 16:37:48 2026 GMT
  host: www.snapeda.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snapmagic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SnapMagic, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SnapMagic
provider_slug: snapmagic
slug: snapmagic-domain-security
source_filename: snapmagic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.snapmagic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:07:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.snapeda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 16:37:48 2026 GMT\n  hsts: false\ndomains:\n- domain: snapmagic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: snapeda.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapmagic/refs/heads/main/security/snapmagic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Electronics
- PCB Design
- Electronic Design Automation
- CAD
- Components
- Symbols
- Footprints
- Hardware
- Semiconductors
- AI
- Search
---
