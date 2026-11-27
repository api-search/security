---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: choosehelp.com
  spf: true
hosts:
- cert_expires: Jan 29 02:26:40 2027 GMT
  host: choosehelp.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ChooseHelp.com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChooseHelp.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ChooseHelp.com
provider_slug: choosehelp-com
slug: choosehelp-com-domain-security
source_filename: choosehelp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: choosehelp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 02:26:40 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: choosehelp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/choosehelp-com/security/choosehelp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Addiction Treatment
- Mental Health
- Healthcare
- Directory
- Therapists
- MCP
---
