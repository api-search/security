---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iodinesoftware.com
  spf: true
hosts:
- cert_expires: Aug 29 11:49:50 2026 GMT
  host: iodinesoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iodine Software Waystar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iodine Software (Waystar), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Iodine Software (Waystar)
provider_slug: iodine-software-waystar
slug: iodine-software-waystar-domain-security
source_filename: iodine-software-waystar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iodinesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 11:49:50 2026 GMT\n  hsts: false\ndomains:\n- domain: iodinesoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iodine-software-waystar/refs/heads/main/security/iodine-software-waystar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Clinical Documentation Integrity
- Revenue Cycle Management
- Artificial Intelligence
- Machine Learning
- Health IT
- EHR Integration
---
