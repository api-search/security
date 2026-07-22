---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tastemade.com
  spf: true
hosts:
- cert_expires: Aug 22 01:50:38 2026 GMT
  host: www.tastemade.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tastemade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tastemade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tastemade
provider_slug: tastemade
slug: tastemade-domain-security
source_filename: tastemade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tastemade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 01:50:38 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: tastemade.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tastemade/refs/heads/main/security/tastemade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Video
- Streaming
- Food
- Travel
- Lifestyle
- Content
- Entertainment
---
