---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brunswick.com
  spf: true
hosts:
- cert_expires: Sep  2 08:01:47 2026 GMT
  host: www.brunswick.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brunswick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brunswick Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brunswick Corporation
provider_slug: brunswick
slug: brunswick-domain-security
source_filename: brunswick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brunswick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 08:01:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brunswick.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brunswick/refs/heads/main/security/brunswick-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Boat Manufacturing
- Boating
- Connectivity
- Electrification
- Marine
- Marine Electronics
- Marine Propulsion
- Recreation
- Fortune 1000
---
