---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hilos.sh
  spf: true
hosts:
- cert_expires: Jan 13 23:52:50 2027 GMT
  host: hilos.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: hilos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hilos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: hilos
provider_slug: hilos-sh
slug: hilos-sh-domain-security
source_filename: hilos-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hilos.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:52:50 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hilos.sh\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hilos-sh/security/hilos-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Artificial Intelligence
- Chat
- Developer Tools
- Productivity
---
