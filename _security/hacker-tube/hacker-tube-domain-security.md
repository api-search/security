---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hacker-tube.com
  spf: true
hosts:
- cert_expires: Jan 31 15:00:29 2027 GMT
  host: hacker-tube.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HackerTube AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HackerTube AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HackerTube AI
provider_slug: hacker-tube
slug: hacker-tube-domain-security
source_filename: hacker-tube-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hacker-tube.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 15:00:29 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: hacker-tube.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hacker-tube/security/hacker-tube-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Video
- Community
- Curated
- Programming
- Artificial Intelligence
- Science
---
