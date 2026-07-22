---
description: ''
domains:
- caa:
  - alb-6t9bperiqxmkyjlfb9.ap-southeast-1.alb.aliyuncsslbintl.com.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: urbanrevivo.com
  spf: true
hosts:
- cert_expires: Oct  4 14:47:33 2026 GMT
  host: global.urbanrevivo.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urban Revivo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urban Revivo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Urban Revivo
provider_slug: urban-revivo
slug: urban-revivo-domain-security
source_filename: urban-revivo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: global.urbanrevivo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:47:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: urbanrevivo.com\n  dnssec: true\n  caa:\n  - alb-6t9bperiqxmkyjlfb9.ap-southeast-1.alb.aliyuncsslbintl.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urban-revivo/refs/heads/main/security/urban-revivo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Fashion
- Retail
- eCommerce
- Apparel
- Agentic Commerce
---
