---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aistarfish.com
  spf: true
hosts:
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: aistarfish.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Aistarfish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aistarfish, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: aistarfish
provider_slug: aistarfish
slug: aistarfish-domain-security
source_filename: aistarfish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aistarfish.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aistarfish.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aistarfish/refs/heads/main/security/aistarfish-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Healthcare
- Digital Health
- Oncology
- Patient Management
- Mobile Apps
- China
---
