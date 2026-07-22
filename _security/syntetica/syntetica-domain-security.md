---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: syntetica.co
  spf: true
hosts:
- cert_expires: Oct  1 04:28:08 2026 GMT
  host: www.syntetica.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Syntetica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syntetica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Syntetica
provider_slug: syntetica
slug: syntetica-domain-security
source_filename: syntetica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.syntetica.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:28:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: syntetica.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syntetica/refs/heads/main/security/syntetica-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Sustainability
- Cleantech
- Recycling
- Materials Science
- Textiles
- Circular Economy
- Green Chemistry
---
