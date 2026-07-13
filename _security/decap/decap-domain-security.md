---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: decapcms.org
  spf: true
hosts:
- cert_expires: Sep 26 06:56:54 2026 GMT
  host: decapcms.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Decap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Decap CMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Decap CMS
provider_slug: decap
slug: decap-domain-security
source_filename: decap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decapcms.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 06:56:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: decapcms.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decap/refs/heads/main/security/decap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Headless CMS
- Git-based CMS
- Content Management
- Static Site Generator
- JAMstack
- Open Source
- Editorial Workflow
---
