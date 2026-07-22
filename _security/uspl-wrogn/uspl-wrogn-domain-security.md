---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wrogn.com
  spf: true
hosts:
- cert_expires: Sep 17 12:06:33 2026 GMT
  host: wrogn.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uspl Wrogn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for USPL Wrogn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: USPL Wrogn
provider_slug: uspl-wrogn
slug: uspl-wrogn-domain-security
source_filename: uspl-wrogn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wrogn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 12:06:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: wrogn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uspl-wrogn/refs/heads/main/security/uspl-wrogn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Fashion
- Apparel
- eCommerce
- Retail
- India
- Agentic Commerce
- MCP
---
