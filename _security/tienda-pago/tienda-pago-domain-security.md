---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tiendapago.com
  spf: true
hosts:
- cert_expires: Dec 31 12:49:27 2026 GMT
  host: tiendapago.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tienda Pago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tienda Pago, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tienda Pago
provider_slug: tienda-pago
slug: tienda-pago-domain-security
source_filename: tienda-pago-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tiendapago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 12:49:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tiendapago.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tienda-pago/refs/heads/main/security/tienda-pago-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Lending
- Fintech
- Payments
- Working Capital
- Buy Now Pay Later
- Mexico
- Peru
- Small Business
---
