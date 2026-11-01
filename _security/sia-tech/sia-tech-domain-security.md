---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sia.tech
  spf: true
hosts:
- cert_expires: Jan 17 19:29:05 2027 GMT
  host: sia.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sia Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sia
provider_slug: sia-tech
slug: sia-tech-domain-security
source_filename: sia-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sia.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:29:05 2027 GMT\n  hsts: false\ndomains:\n- domain: sia.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/sia-tech/security/sia-tech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Decentralized Storage
- Cloud Storage
- Blockchain
- Open Source
- Developer Tools
---
