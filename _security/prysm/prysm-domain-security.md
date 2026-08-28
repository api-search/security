---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prysm.com
  spf: true
hosts:
- cert_expires: Nov 12 13:03:44 2026 GMT
  host: www.prysm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prysm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prysm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Prysm
provider_slug: prysm
slug: prysm-domain-security
source_filename: prysm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prysm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 13:03:44 2026 GMT\n  hsts: false\ndomains:\n- domain: prysm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prysm/refs/heads/main/security/prysm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Collaboration
- Visual Collaboration
- Digital Workplace
- Displays
- Display Technology
- Hardware
- Meetings
- Whiteboarding
- Enterprise Software
- Unified Communications
---
