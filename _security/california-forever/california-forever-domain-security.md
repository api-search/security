---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: californiaforever.com
  spf: true
hosts:
- cert_expires: Sep 10 12:02:23 2026 GMT
  host: californiaforever.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: California Forever Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for California Forever, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: California Forever
provider_slug: california-forever
slug: california-forever-domain-security
source_filename: california-forever-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: californiaforever.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 12:02:23 2026 GMT\n  hsts: false\ndomains:\n- domain: californiaforever.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/california-forever/refs/heads/main/security/california-forever-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Urban Development
- Construction
- Manufacturing
- Infrastructure
- California
- Venture Backed
---
