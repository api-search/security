---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: archive.org
  spf: true
hosts:
- cert_expires: Feb  9 22:02:42 2027 GMT
  host: archive.org
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Internet Archive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Internet Archive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Internet Archive
provider_slug: internet-archive
slug: internet-archive-domain-security
source_filename: internet-archive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: archive.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 22:02:42 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: archive.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/internet-archive/refs/heads/main/security/internet-archive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Library
- Non-Profit
- Archival
- Open Access
- Research
---
