---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rohnelt.dev
  spf: true
hosts:
- cert_expires: Jan 10 10:01:13 2027 GMT
  host: rohnelt.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rohnelt Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for rohnelt-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: rohnelt-dev
provider_slug: rohnelt-dev
slug: rohnelt-dev-domain-security
source_filename: rohnelt-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rohnelt.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 10:01:13 2027 GMT\n  hsts: false\ndomains:\n- domain: rohnelt.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/rohnelt-dev/security/rohnelt-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Software Engineering
- Operations
- Consulting
- Brazil
- Logistics
- Industry
---
