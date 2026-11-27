---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mirondo.net
  spf: false
hosts:
- cert_expires: Feb  4 16:18:47 2027 GMT
  host: mirondo.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mirondo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mirondo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mirondo
provider_slug: mirondo-net
slug: mirondo-net-domain-security
source_filename: mirondo-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mirondo.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 16:18:47 2027 GMT\n  hsts: false\ndomains:\n- domain: mirondo.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mirondo-net/security/mirondo-net-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
