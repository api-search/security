---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sigit.si
  spf: false
hosts:
- cert_expires: Jan  7 23:17:03 2027 GMT
  host: sigit.si
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sigit Si Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sigit-si, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: sigit-si
provider_slug: sigit-si
slug: sigit-si-domain-security
source_filename: sigit-si-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sigit.si\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:17:03 2027 GMT\n  hsts: false\ndomains:\n- domain: sigit.si\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sigit-si/security/sigit-si-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Git Hosting
- AI
- Version Control
- Model Storage
- Open Source
---
