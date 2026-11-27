---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parahuman.co
  spf: true
hosts:
- cert_expires: Feb 13 10:29:09 2027 GMT
  host: parahuman.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Parahuman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parahuman, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Parahuman
provider_slug: parahuman-co
slug: parahuman-co-domain-security
source_filename: parahuman-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parahuman.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 10:29:09 2027 GMT\n  hsts: false\ndomains:\n- domain: parahuman.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/parahuman-co/security/parahuman-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Social Listening
- Brand Monitoring
- Software-as-a-Service
- Marketing
---
