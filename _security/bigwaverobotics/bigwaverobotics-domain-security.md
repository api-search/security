---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bigwaverobotics.com
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: bigwaverobotics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bigwaverobotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bigwaverobotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bigwaverobotics
provider_slug: bigwaverobotics
slug: bigwaverobotics-domain-security
source_filename: bigwaverobotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bigwaverobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bigwaverobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigwaverobotics/refs/heads/main/security/bigwaverobotics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Robotics
- Artificial Intelligence
- Industrial Automation
- Manufacturing
---
