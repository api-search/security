---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getfirmament.com
  spf: false
hosts:
- cert_expires: Jan  7 03:30:53 2027 GMT
  host: getfirmament.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firmament Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firmament, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Firmament
provider_slug: getfirmament-com
slug: getfirmament-com-domain-security
source_filename: getfirmament-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getfirmament.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 03:30:53 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: getfirmament.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getfirmament-com/security/getfirmament-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Automation
- Agents
- Workflows
---
