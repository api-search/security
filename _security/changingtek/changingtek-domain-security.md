---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: changingtek.com
  spf: false
hosts:
- cert_expires: Dec 14 07:20:46 2026 GMT
  host: en.changingtek.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Changingtek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Changingtek, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Changingtek
provider_slug: changingtek
slug: changingtek-domain-security
source_filename: changingtek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.changingtek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 07:20:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: changingtek.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/changingtek/refs/heads/main/security/changingtek-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Robotics
- Automation
- Manufacturing
- AI
---
