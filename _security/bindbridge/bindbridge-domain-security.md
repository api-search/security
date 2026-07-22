---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bindbridge.com
  spf: true
hosts:
- cert_expires: Aug 21 21:22:14 2026 GMT
  host: bindbridge.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bindbridge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bindbridge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bindbridge
provider_slug: bindbridge
slug: bindbridge-domain-security
source_filename: bindbridge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bindbridge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 21:22:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bindbridge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bindbridge/refs/heads/main/security/bindbridge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- Biotechnology
- Artificial Intelligence
- Molecular Discovery
- Crop Protection
- Drug Discovery
---
