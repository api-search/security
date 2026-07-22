---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kaizntree.com
  spf: true
hosts:
- cert_expires: Sep 25 00:47:13 2026 GMT
  host: kaizntree.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kaizntree Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaizntree Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kaizntree Inc.
provider_slug: kaizntree-inc
slug: kaizntree-inc-domain-security
source_filename: kaizntree-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kaizntree.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 00:47:13 2026 GMT\n  hsts: null\ndomains:\n- domain: kaizntree.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaizntree-inc/refs/heads/main/security/kaizntree-inc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Operations
- ERP
- Inventory Management
- CPG
- Consumer Packaged Goods
- Supply Chain
- Manufacturing
- AI Agents
---
