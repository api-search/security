---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: asianrecs.com
  spf: false
hosts:
- cert_expires: Dec 25 09:23:12 2026 GMT
  host: asianrecs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asian Recs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asian Recs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Asian Recs
provider_slug: asianrecs-com
slug: asianrecs-com-domain-security
source_filename: asianrecs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asianrecs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 09:23:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: asianrecs.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/asianrecs-com/security/asianrecs-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Restaurant
- Food
- Rankings
- Asian Cuisine
---
