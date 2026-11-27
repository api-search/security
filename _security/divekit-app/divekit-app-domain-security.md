---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: divekit.app
  spf: true
hosts:
- cert_expires: Jan  1 15:09:52 2027 GMT
  host: divekit.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dive Kit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dive Kit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dive Kit
provider_slug: divekit-app
slug: divekit-app-domain-security
source_filename: divekit-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: divekit.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 15:09:52 2027 GMT\n  hsts: false\ndomains:\n- domain: divekit.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/divekit-app/security/divekit-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Diving
- Decompression
- Mobile App
- Tools
---
