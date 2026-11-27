---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ego.dog
  spf: true
hosts:
- cert_expires: Jan 11 07:21:26 2027 GMT
  host: ego.dog
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ego Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ego, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ego
provider_slug: ego-dog
slug: ego-dog-domain-security
source_filename: ego-dog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ego.dog\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 07:21:26 2027 GMT\n  hsts: false\ndomains:\n- domain: ego.dog\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ego-dog/security/ego-dog-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- LinkedIn
- Content Generation
- Social Media
- Marketing
---
