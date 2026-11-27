---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: memofs.dev
  spf: false
hosts:
- cert_expires: Feb  2 11:54:30 2027 GMT
  host: memofs.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: memofs-dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for memofs-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: memofs-dev
provider_slug: memofs-dev
slug: memofs-dev-domain-security
source_filename: memofs-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memofs.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 11:54:30 2027 GMT\n  hsts: null\ndomains:\n- domain: memofs.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/memofs-dev/security/memofs-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
