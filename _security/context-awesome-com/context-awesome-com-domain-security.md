---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: context-awesome.com
  spf: false
hosts:
- cert_expires: Jan 28 00:58:33 2027 GMT
  host: context-awesome.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Context Awesome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Context Awesome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Context Awesome
provider_slug: context-awesome-com
slug: context-awesome-com-domain-security
source_filename: context-awesome-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: context-awesome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 00:58:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: context-awesome.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/context-awesome-com/security/context-awesome-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Data
- Tools
- Community
- MCP
---
