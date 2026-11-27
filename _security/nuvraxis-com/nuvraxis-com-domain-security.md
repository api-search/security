---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nuvraxis.com
  spf: true
hosts:
- cert_expires: Feb  5 15:25:34 2027 GMT
  host: nuvraxis.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nuvraxis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuvraxis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nuvraxis
provider_slug: nuvraxis-com
slug: nuvraxis-com-domain-security
source_filename: nuvraxis-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nuvraxis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 15:25:34 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: nuvraxis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nuvraxis-com/security/nuvraxis-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Full-stack Development
- AI Agents
- Health Tech
- Fintech
- Cloud
- AI Consulting
- Document AI
---
