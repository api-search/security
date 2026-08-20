---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: evergreentgn.com
  spf: true
hosts:
- cert_expires: Oct 23 13:24:51 2026 GMT
  host: www.evergreentgn.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evergreen Theragnostics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evergreen Theragnostics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Evergreen Theragnostics
provider_slug: evergreen-theragnostics
slug: evergreen-theragnostics-domain-security
source_filename: evergreen-theragnostics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evergreentgn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 13:24:51 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: evergreentgn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evergreen-theragnostics/refs/heads/main/security/evergreen-theragnostics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Pharmaceuticals
- Life Sciences
- Manufacturing
- Radiopharmaceuticals
- Oncology
- Contract Manufacturing
- Medical Imaging
---
