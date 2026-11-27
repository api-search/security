---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: alexandria-archive.com
  spf: true
hosts:
- cert_expires: Jan 31 12:04:31 2027 GMT
  host: alexandria-archive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 12:04:31 2027 GMT
  host: www.alexandria-archive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Alexandria Archive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alexandria Archive, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Alexandria Archive
provider_slug: alexandria-archive-com
slug: alexandria-archive-com-domain-security
source_filename: alexandria-archive-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alexandria-archive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 12:04:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.alexandria-archive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 12:04:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alexandria-archive.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/alexandria-archive-com/security/alexandria-archive-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Archives
- History
- Egypt
- Digital Preservation
- Culture
- Photography
- Community
---
