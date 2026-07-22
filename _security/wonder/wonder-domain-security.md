---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wonder.com
  spf: true
hosts:
- cert_expires: Sep 20 17:48:32 2026 GMT
  host: www.wonder.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wonder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wonder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wonder
provider_slug: wonder
slug: wonder-domain-security
source_filename: wonder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wonder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:48:32 2026 GMT\n  hsts: false\ndomains:\n- domain: wonder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wonder/refs/heads/main/security/wonder-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Food
- Delivery
- Marketplace
---
