---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tepali.com
  spf: true
hosts:
- cert_expires: Sep 28 13:54:06 2026 GMT
  host: www.tepali.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tepali Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tepali, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tepali
provider_slug: tepali
slug: tepali-domain-security
source_filename: tepali-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tepali.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:54:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tepali.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tepali/refs/heads/main/security/tepali-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health
- Medical Spa
- Aesthetics
- Wellness
- Practice Management
- Artificial Intelligence
- SaaS
- Scheduling
- Patient CRM
---
