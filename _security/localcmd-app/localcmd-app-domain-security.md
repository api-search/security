---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: localcmd.app
  spf: true
hosts:
- cert_expires: Jan  2 10:29:15 2027 GMT
  host: localcmd.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Local Commander Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Local Commander, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Local Commander
provider_slug: localcmd-app
slug: localcmd-app-domain-security
source_filename: localcmd-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: localcmd.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 10:29:15 2027 GMT\n  hsts: false\ndomains:\n- domain: localcmd.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/localcmd-app/security/localcmd-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Remote-Computing
- Automation
- Productivity
- Company
---
