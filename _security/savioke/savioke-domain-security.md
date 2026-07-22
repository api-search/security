---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: savioke.com
  spf: true
hosts:
- cert_expires: Oct  9 10:56:48 2026 GMT
  host: savioke.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Savioke Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Savioke, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Savioke
provider_slug: savioke
slug: savioke-domain-security
source_filename: savioke-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: savioke.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 10:56:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: savioke.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savioke/refs/heads/main/security/savioke-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Frontier Tech
- Robotics
- Autonomous Robots
- Delivery Robots
- Automation
- Hospitality
---
