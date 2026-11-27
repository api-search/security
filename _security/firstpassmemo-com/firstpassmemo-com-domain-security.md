---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: firstpassmemo.com
  spf: true
hosts:
- cert_expires: Jan  5 01:16:45 2027 GMT
  host: firstpassmemo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: firstpassmemo-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for firstpassmemo-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: firstpassmemo-com
provider_slug: firstpassmemo-com
slug: firstpassmemo-com-domain-security
source_filename: firstpassmemo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firstpassmemo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 01:16:45 2027 GMT\n  hsts: false\ndomains:\n- domain: firstpassmemo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/firstpassmemo-com/security/firstpassmemo-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Red‑flag checker
- Business For Sale
- Deal screening
- Buyer tools
---
