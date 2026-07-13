---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: modine.com
  spf: true
hosts:
- cert_expires: Aug 31 03:35:18 2026 GMT
  host: www.modine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.modine.com
  https: false
- host: api.modine.com
  https: false
kind: domain-security
layout: security
method: probed
name: Modine Manufacturing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modine Manufacturing, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Modine Manufacturing
provider_slug: modine-manufacturing
slug: modine-manufacturing-domain-security
source_filename: modine-manufacturing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.modine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 03:35:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.modine.com\n  https: false\n- host: api.modine.com\n  https: false\ndomains:\n- domain: modine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modine-manufacturing/refs/heads/main/security/modine-manufacturing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Thermal Management
- Automotive
- HVAC
---
