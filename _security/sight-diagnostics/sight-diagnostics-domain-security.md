---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sightdx.com
  spf: true
hosts:
- cert_expires: Nov 23 01:52:47 2026 GMT
  host: www.sightdx.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sight Diagnostics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sight Diagnostics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sight Diagnostics
provider_slug: sight-diagnostics
slug: sight-diagnostics-domain-security
source_filename: sight-diagnostics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sightdx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 01:52:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: sightdx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sight-diagnostics/refs/heads/main/security/sight-diagnostics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Medical Devices
- Diagnostics
- Hematology
- Point of Care
- Laboratory
- Artificial Intelligence
- Computer-Vision
- Israel
---
