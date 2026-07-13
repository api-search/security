---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: loomly.com
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: www.loomly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.loomly.com
  https: false
kind: domain-security
layout: security
method: probed
name: Loomly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loomly, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Loomly
provider_slug: loomly
slug: loomly-domain-security
source_filename: loomly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.loomly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: false\n- host: api.loomly.com\n  https: false\ndomains:\n- domain: loomly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loomly/refs/heads/main/security/loomly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social Media
- Content Calendar
- Scheduling
- Approval Workflows
- Analytics
- Brand Management
- Publishing
- Community Management
---
