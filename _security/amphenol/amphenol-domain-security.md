---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amphenol.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amphenol-industrial.com
  spf: true
hosts:
- cert_expires: Nov  9 09:57:46 2026 GMT
  host: www.amphenol.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 07:48:07 2026 GMT
  host: amphenol-industrial.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 07:37:15 2026 GMT
  host: amphenol-automotive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amphenol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amphenol, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Amphenol
provider_slug: amphenol
slug: amphenol-domain-security
source_filename: amphenol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amphenol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 09:57:46 2026 GMT\n  hsts: null\n- host: amphenol-industrial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 07:48:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: amphenol-automotive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 07:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amphenol.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: amphenol-industrial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amphenol/refs/heads/main/security/amphenol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Electronic Connectors
- Interconnect Systems
- Fiber Optics
- Sensors
- Aerospace
- Automotive
- Defense
- Manufacturing
- Fortune 500
---
