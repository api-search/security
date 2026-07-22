---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pitzi.com.br
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: pitzi.com.br
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pitzi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pitzi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pitzi
provider_slug: pitzi
slug: pitzi-domain-security
source_filename: pitzi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pitzi.com.br\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: pitzi.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pitzi/refs/heads/main/security/pitzi-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fintech
- Insurtech
- Insurance
- Mobile
- Device Protection
- Brazil
- Consumer
---
