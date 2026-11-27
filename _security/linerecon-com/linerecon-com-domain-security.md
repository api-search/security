---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: linerecon.com
  spf: true
hosts:
- cert_expires: Feb 15 04:04:41 2027 GMT
  host: linerecon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LineRecon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LineRecon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LineRecon
provider_slug: linerecon-com
slug: linerecon-com-domain-security
source_filename: linerecon-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linerecon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 04:04:41 2027 GMT\n  hsts: false\ndomains:\n- domain: linerecon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/linerecon-com/security/linerecon-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Software-as-a-Service
- Procurement
- Finance
- Document-Comparison
- Automation
---
