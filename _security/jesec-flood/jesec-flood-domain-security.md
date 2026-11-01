---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: js.org
  spf: true
hosts:
- cert_expires: Jan 11 05:51:36 2027 GMT
  host: flood.js.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jesec Flood Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flood, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Flood
provider_slug: jesec-flood
slug: jesec-flood-domain-security
source_filename: jesec-flood-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flood.js.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 05:51:36 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: js.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/jesec-flood/security/jesec-flood-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- OpenSource
- Torrent
- WebUI
- JavaScript
---
