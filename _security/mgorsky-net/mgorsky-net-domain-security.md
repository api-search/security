---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mgorsky.net
  spf: true
hosts:
- cert_expires: Dec 24 19:33:48 2026 GMT
  host: mgorsky.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mikael Alemu Gorsky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mikael Alemu Gorsky, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mikael Alemu Gorsky
provider_slug: mgorsky-net
slug: mgorsky-net-domain-security
source_filename: mgorsky-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mgorsky.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 19:33:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mgorsky.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mgorsky-net/security/mgorsky-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Research
- Artificial Intelligence
- Software Engineering
- Open Source
- Personal Site
---
