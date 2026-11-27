---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lugara.me
  spf: true
hosts:
- cert_expires: Feb 13 22:22:50 2027 GMT
  host: lugara.me
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lugara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lugara, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lugara
provider_slug: lugara-me
slug: lugara-me-domain-security
source_filename: lugara-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lugara.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 22:22:50 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: lugara.me\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lugara-me/security/lugara-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Travel
- Privacy
- DataInsights
- Nomads
- Explorer
---
