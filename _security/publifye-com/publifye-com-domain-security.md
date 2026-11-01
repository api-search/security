---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: publifye.com
  spf: true
hosts:
- cert_expires: Nov 30 13:37:56 2026 GMT
  host: publifye.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Publifye Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for publifye-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: publifye-com
provider_slug: publifye-com
slug: publifye-com-domain-security
source_filename: publifye-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: publifye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 13:37:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: publifye.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/publifye-com/security/publifye-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Bible
- Publishing
- AI
- Norway
- Data
---
