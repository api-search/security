---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pagelet.host
  spf: true
hosts:
- cert_expires: Feb 13 23:51:44 2027 GMT
  host: pagelet.host
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pagelet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pagelet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pagelet
provider_slug: pagelet-host
slug: pagelet-host-domain-security
source_filename: pagelet-host-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagelet.host\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:51:44 2027 GMT\n  hsts: false\ndomains:\n- domain: pagelet.host\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pagelet-host/security/pagelet-host-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hosting
- HTML
- Artificial Intelligence
- Free
- Static Sites
---
