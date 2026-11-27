---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: gridgarden.eu
  spf: true
hosts:
- cert_expires: Jan  6 08:44:00 2027 GMT
  host: gridgarden.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GridGarden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GridGarden, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: GridGarden
provider_slug: gridgarden-eu
slug: gridgarden-eu-domain-security
source_filename: gridgarden-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gridgarden.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 08:44:00 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gridgarden.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gridgarden-eu/security/gridgarden-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Gardening
- Design
- Software-as-a-Service
- EU
---
