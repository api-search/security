---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hrblock.com
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: www.hrblock.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.hrblock.com
  https: false
- host: api.hrblock.com
  https: false
kind: domain-security
layout: security
method: probed
name: Hanr Block Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for H&R Block, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: H&R Block
provider_slug: hanr-block
slug: hanr-block-domain-security
source_filename: hanr-block-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hrblock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\n- host: developer.hrblock.com\n  https: false\n- host: api.hrblock.com\n  https: false\ndomains:\n- domain: hrblock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hanr-block/refs/heads/main/security/hanr-block-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Tax Preparation
- Financial Services
- Fortune 1000
---
