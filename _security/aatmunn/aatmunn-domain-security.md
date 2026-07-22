---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aatmunn.com
  spf: true
hosts:
- cert_expires: Sep 19 23:31:45 2026 GMT
  host: aatmunn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aatmunn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aatmunn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aatmunn
provider_slug: aatmunn
slug: aatmunn-domain-security
source_filename: aatmunn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aatmunn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:31:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aatmunn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aatmunn/refs/heads/main/security/aatmunn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Worker Safety
- Industrial IoT
- Asset Intelligence
- Connected Worker
- Occupational Safety
- Compliance
- Frontline Workers
---
