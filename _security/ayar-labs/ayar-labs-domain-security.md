---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ayarlabs.com
  spf: true
hosts:
- cert_expires: Sep  8 05:28:45 2026 GMT
  host: ayarlabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ayar Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ayar Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ayar Labs
provider_slug: ayar-labs
slug: ayar-labs-domain-security
source_filename: ayar-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ayarlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 05:28:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ayarlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ayar-labs/refs/heads/main/security/ayar-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Silicon Photonics
- Co-Packaged Optics
- Optical I/O
- Semiconductors
- AI Infrastructure
- GPU Interconnect
- Hardware
---
