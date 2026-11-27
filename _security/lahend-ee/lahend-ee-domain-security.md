---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: lahend.ee
  spf: true
hosts:
- cert_expires: Feb 12 15:47:32 2027 GMT
  host: lahend.ee
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: lahend.ee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lahend.ee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: lahend.ee
provider_slug: lahend-ee
slug: lahend-ee-domain-security
source_filename: lahend-ee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lahend.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 15:47:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lahend.ee\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lahend-ee/security/lahend-ee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Legal Tech
- Estonia
- Open Data
- CourtDecisions
---
