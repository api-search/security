---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cloudresume.io
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: cloudresume.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: cloudresume.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cloudresume.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: cloudresume.io
provider_slug: cloudresume-io
slug: cloudresume-io-domain-security
source_filename: cloudresume-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudresume.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cloudresume.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cloudresume-io/security/cloudresume-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Resume
- Resume Builder
- Careers
- Artificial Intelligence
- Cover Letters
- JSON Resume
- MCP
---
