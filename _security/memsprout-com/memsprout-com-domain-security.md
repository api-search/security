---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: memsprout.com
  spf: false
hosts:
- cert_expires: Jan  6 20:09:26 2027 GMT
  host: memsprout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Memsprout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memsprout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Memsprout
provider_slug: memsprout-com
slug: memsprout-com-domain-security
source_filename: memsprout-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memsprout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 20:09:26 2027 GMT\n  hsts: false\ndomains:\n- domain: memsprout.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/memsprout-com/security/memsprout-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Collaboration
- Knowledge Management
- Team Productivity
---
