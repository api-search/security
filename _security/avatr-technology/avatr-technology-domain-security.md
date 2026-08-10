---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: avatr.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: avatr.hk
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.avatr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 03:05:13 2026 GMT
  host: www.avatr.hk
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avatr Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avatr Technology, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Avatr Technology
provider_slug: avatr-technology
slug: avatr-technology-domain-security
source_filename: avatr-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avatr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\n- host: www.avatr.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 03:05:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: avatr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: avatr.hk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avatr-technology/refs/heads/main/security/avatr-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Automotive
- Electric Vehicles
- Smart Cockpit
- Autonomous Driving
- Manufacturing
- China
- Consumer
---
