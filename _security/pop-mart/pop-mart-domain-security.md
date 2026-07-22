---
description: ''
domains:
- caa:
  - popmart.com.cdn.cloudflare.net.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: popmart.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: popmart.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pop Mart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pop Mart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Pop Mart
provider_slug: pop-mart
slug: pop-mart-domain-security
source_filename: pop-mart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: popmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: popmart.com\n  dnssec: true\n  caa:\n  - popmart.com.cdn.cloudflare.net.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pop-mart/refs/heads/main/security/pop-mart-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Consumer
- Retail
- E-commerce
- Collectibles
- Toys
- Consumer Products
---
