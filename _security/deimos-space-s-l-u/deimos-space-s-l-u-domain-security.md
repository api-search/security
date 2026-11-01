---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: indragroup.com
  spf: true
hosts:
- cert_expires: Apr 15 23:59:59 2027 GMT
  host: space.indragroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deimos Space S L U Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DEIMOS Space S.L.U., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DEIMOS Space S.L.U.
provider_slug: deimos-space-s-l-u
slug: deimos-space-s-l-u-domain-security
source_filename: deimos-space-s-l-u-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: space.indragroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: indragroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/deimos-space-s-l-u/security/deimos-space-s-l-u-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
