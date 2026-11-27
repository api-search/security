---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: learnthedao.com
  spf: true
hosts:
- cert_expires: Jan 25 09:23:12 2027 GMT
  host: learnthedao.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Learn the Dao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Learn the Dao, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Learn the Dao
provider_slug: learnthedao-com
slug: learnthedao-com-domain-security
source_filename: learnthedao-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learnthedao.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 09:23:12 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: learnthedao.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/learnthedao-com/security/learnthedao-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
