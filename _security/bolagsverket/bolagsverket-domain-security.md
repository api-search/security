---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bolagsverket.se
  spf: true
hosts:
- cert_expires: Feb 25 10:31:58 2027 GMT
  host: bolagsverket.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bolagsverket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bolagsverket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bolagsverket
provider_slug: bolagsverket
slug: bolagsverket-domain-security
source_filename: bolagsverket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bolagsverket.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 10:31:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bolagsverket.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolagsverket/refs/heads/main/security/bolagsverket-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Government
- Registry
- Sweden
- Business
---
