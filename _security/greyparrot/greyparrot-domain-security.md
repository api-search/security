---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greyparrot.ai
  spf: true
hosts:
- cert_expires: Sep 15 14:07:06 2026 GMT
  host: www.greyparrot.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greyparrot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greyparrot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Greyparrot
provider_slug: greyparrot
slug: greyparrot-domain-security
source_filename: greyparrot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greyparrot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:07:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: greyparrot.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greyparrot/refs/heads/main/security/greyparrot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Computer Vision
- Waste Management
- Recycling
- Sustainability
- Circular Economy
- Analytics
- Materials Recovery
- Environmental
---
