---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: birentech.com
  spf: true
hosts:
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: www.birentech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Birentechnology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Birentechnology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Birentechnology
provider_slug: birentechnology
slug: birentechnology-domain-security
source_filename: birentechnology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.birentech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: birentech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/birentechnology/refs/heads/main/security/birentechnology-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Semiconductors
- Artificial Intelligence
- GPU
- Cloud
---
