---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zbiotics.com
  spf: true
hosts:
- cert_expires: Oct 26 18:33:34 2026 GMT
  host: zbiotics.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zbiotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZBiotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ZBiotics
provider_slug: zbiotics
slug: zbiotics-domain-security
source_filename: zbiotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zbiotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 18:33:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: zbiotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zbiotics/refs/heads/main/security/zbiotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biotechnology
- Probiotics
- Consumer Health
- Direct to Consumer
- E-Commerce
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Shopify
- Company
---
