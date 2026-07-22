---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lincolnelectric.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: www.lincolnelectric.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lincoln Electric Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lincoln Electric Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lincoln Electric Holdings
provider_slug: lincoln-electric-holdings
slug: lincoln-electric-holdings-domain-security
source_filename: lincoln-electric-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lincolnelectric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lincolnelectric.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lincoln-electric-holdings/refs/heads/main/security/lincoln-electric-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cutting
- Industrial
- Manufacturing
- Robotics
- Welding
- Fortune 1000
---
