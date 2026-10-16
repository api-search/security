---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: byeaerospace.com
  spf: true
hosts:
- cert_expires: Dec  1 11:54:27 2026 GMT
  host: www.byeaerospace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Byeaerospace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Byeaerospace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Byeaerospace
provider_slug: byeaerospace
slug: byeaerospace-domain-security
source_filename: byeaerospace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.byeaerospace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 11:54:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: byeaerospace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byeaerospace/refs/heads/main/security/byeaerospace-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Electric Aviation
- Flight Training
- Training Aircraft
---
