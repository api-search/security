---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: golfcore.org
  spf: true
hosts:
- cert_expires: Jan 12 20:16:28 2027 GMT
  host: golfcore.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GolfCore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GolfCore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: GolfCore
provider_slug: golfcore-org
slug: golfcore-org-domain-security
source_filename: golfcore-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: golfcore.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 20:16:28 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: golfcore.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/golfcore-org/security/golfcore-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Golf
- GPS
- Sports
- Mobile App
---
