---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clarapath.com
  spf: true
hosts:
- cert_expires: Nov  6 00:11:55 2026 GMT
  host: clarapath.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clarapath Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clarapath, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clarapath
provider_slug: clarapath
slug: clarapath-domain-security
source_filename: clarapath-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clarapath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 00:11:55 2026 GMT\n  hsts: false\ndomains:\n- domain: clarapath.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarapath/refs/heads/main/security/clarapath-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Medical Devices
- Robotics
- Pathology
- Histology
- Laboratory Automation
- Diagnostics
- Life Sciences
---
