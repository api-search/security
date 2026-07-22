---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rothys.com
  spf: true
hosts:
- cert_expires: Aug 27 06:59:33 2026 GMT
  host: www.rothys.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rothys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rothys, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rothys
provider_slug: rothys
slug: rothys-domain-security
source_filename: rothys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rothys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 06:59:33 2026 GMT\n  hsts: null\ndomains:\n- domain: rothys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rothys/refs/heads/main/security/rothys-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Footwear
- Fashion
- Retail
- Sustainability
- E-Commerce
- Direct-to-Consumer
- Consumer Goods
- Apparel
---
