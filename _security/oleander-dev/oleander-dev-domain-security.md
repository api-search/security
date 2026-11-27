---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oleander.dev
  spf: true
hosts:
- cert_expires: Feb 14 01:19:18 2027 GMT
  host: oleander.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oleander Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oleander, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Oleander
provider_slug: oleander-dev
slug: oleander-dev-domain-security
source_filename: oleander-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oleander.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 01:19:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oleander.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/oleander-dev/security/oleander-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Warehouse
- AI Agents
- Multi-Engine
- Serverless Compute
- Open Source
---
