---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: maihem.com
  spf: true
hosts:
- cert_expires: Nov 28 16:46:58 2026 GMT
  host: maihem.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Maihem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MAIHEM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: MAIHEM
provider_slug: maihem
slug: maihem-domain-security
source_filename: maihem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maihem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 16:46:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: maihem.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maihem/refs/heads/main/security/maihem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Robotics
- Automation
- Manufacturing
- Welding
---
