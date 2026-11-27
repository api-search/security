---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: laterbase.dev
  spf: true
hosts:
- cert_expires: Jan  1 06:29:32 2027 GMT
  host: laterbase.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Laterbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laterbase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Laterbase
provider_slug: laterbase-dev
slug: laterbase-dev-domain-security
source_filename: laterbase-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laterbase.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 06:29:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: laterbase.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/laterbase-dev/security/laterbase-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Collaboration
- Productivity
- Automation
---
