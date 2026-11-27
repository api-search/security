---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rater8.com
  spf: true
hosts:
- cert_expires: Feb  5 06:42:38 2027 GMT
  host: rater8.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rater8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rater8, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Rater8
provider_slug: rater8
slug: rater8-domain-security
source_filename: rater8-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rater8.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 06:42:38 2027 GMT\n  hsts: false\ndomains:\n- domain: rater8.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/rater8/security/rater8-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Healthcare
- Reputation
- Management
- Software-as-a-Service
- Platform
---
