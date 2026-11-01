---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: geolynx.ee
  spf: false
hosts:
- cert_expires: Dec 29 11:57:01 2026 GMT
  host: geolynx.ee
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Geolynx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geolynx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Geolynx
provider_slug: geolynx
slug: geolynx-domain-security
source_filename: geolynx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geolynx.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 11:57:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: geolynx.ee\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/geolynx/security/geolynx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- GIS
- ESG
- DataHosting
- Training
---
