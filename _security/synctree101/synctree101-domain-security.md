---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: synctree101.com
  spf: false
hosts:
- cert_expires: Dec 17 06:05:11 2026 GMT
  host: synctree101.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Synctree101 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ntuple, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Ntuple
provider_slug: synctree101
slug: synctree101-domain-security
source_filename: synctree101-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synctree101.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 06:05:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: synctree101.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/synctree101/security/synctree101-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Backend
- No-Code
- Software-as-a-Service
---
