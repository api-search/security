---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coverlttr.com
  spf: true
hosts:
- cert_expires: Jan 29 12:34:41 2027 GMT
  host: www.coverlttr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 12:34:41 2027 GMT
  host: mcp.coverlttr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Coverlttr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coverlttr, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coverlttr
provider_slug: coverlttr-com
slug: coverlttr-com-domain-security
source_filename: coverlttr-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coverlttr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 12:34:41 2027 GMT\n  hsts: null\n- host: mcp.coverlttr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 12:34:41 2027 GMT\n  hsts: null\ndomains:\n- domain: coverlttr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/coverlttr-com/security/coverlttr-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cover Letters
- Job Search
- Careers
- Artificial Intelligence
- Writing
- MCP
---
