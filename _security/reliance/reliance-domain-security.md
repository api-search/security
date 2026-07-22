---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reliance.com
  spf: true
hosts:
- cert_expires: Sep 21 06:15:11 2026 GMT
  host: reliance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reliance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reliance, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reliance, Inc.
provider_slug: reliance
slug: reliance-domain-security
source_filename: reliance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reliance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:15:11 2026 GMT\n  hsts: false\ndomains:\n- domain: reliance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reliance/refs/heads/main/security/reliance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Metals
- Manufacturing
- Distribution
- Supply Chain
- Steel
- Aluminum
- Fortune 500
---
