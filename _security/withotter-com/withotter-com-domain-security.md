---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: withotter.com
  spf: true
hosts:
- cert_expires: Jan 25 18:58:18 2027 GMT
  host: withotter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Withotter Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Otter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Otter
provider_slug: withotter-com
slug: withotter-com-domain-security
source_filename: withotter-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withotter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 18:58:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: withotter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/withotter-com/security/withotter-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automation
- Workflow
- Integration
- API
---
