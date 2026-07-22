---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dyna.co
  spf: true
hosts:
- cert_expires: Aug 23 09:37:01 2026 GMT
  host: www.dyna.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dyna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dyna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dyna
provider_slug: dyna
slug: dyna-domain-security
source_filename: dyna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dyna.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 09:37:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dyna.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dyna/refs/heads/main/security/dyna-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Robotics
- Automation
- Embodied AI
- Foundation Models
- Manufacturing
---
