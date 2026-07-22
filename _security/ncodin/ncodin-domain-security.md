---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ncodin.com
  spf: true
hosts:
- cert_expires: Oct  1 04:48:48 2026 GMT
  host: ncodin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ncodin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NcodiN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: NcodiN
provider_slug: ncodin
slug: ncodin-domain-security
source_filename: ncodin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ncodin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:48:48 2026 GMT\n  hsts: false\ndomains:\n- domain: ncodin.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ncodin/refs/heads/main/security/ncodin-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Photonics
- Semiconductors
- Optical Interconnect
- High Performance Computing
- AI Infrastructure
- Deep Tech
- Hardware
---
