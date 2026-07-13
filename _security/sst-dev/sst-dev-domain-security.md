---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sst.dev
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: sst.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sst Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SST, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SST
provider_slug: sst-dev
slug: sst-dev-domain-security
source_filename: sst-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sst.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: sst.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sst-dev/refs/heads/main/security/sst-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Serverless
- Infrastructure as Code
- Cloudflare
- TypeScript
- Full-Stack
- Functions
- Containers
- Open Source
- Framework
---
