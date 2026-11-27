---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: forks.world
  spf: false
hosts:
- cert_expires: Jan  8 07:25:07 2027 GMT
  host: forks.world
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: forks-world Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for forks-world, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: forks-world
provider_slug: forks-world
slug: forks-world-domain-security
source_filename: forks-world-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forks.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 07:25:07 2027 GMT\n  hsts: null\ndomains:\n- domain: forks.world\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/forks-world/security/forks-world-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
