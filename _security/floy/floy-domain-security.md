---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: floy.com
  spf: true
hosts:
- cert_expires: Sep 10 15:36:29 2026 GMT
  host: www.floy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Floy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Floy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Floy
provider_slug: floy
slug: floy-domain-security
source_filename: floy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.floy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:36:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: floy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/floy/refs/heads/main/security/floy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Medical Imaging
- Radiology
- Artificial Intelligence
- Diagnostics
- Clinical Decision Support
- Medical Devices
---
