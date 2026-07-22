---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: melonn.com
  spf: true
hosts:
- cert_expires: Sep 16 01:17:38 2026 GMT
  host: www.melonn.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Melonn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Melonn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Melonn
provider_slug: melonn
slug: melonn-domain-security
source_filename: melonn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.melonn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:17:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: melonn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/melonn/refs/heads/main/security/melonn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fulfillment
- Logistics
- Ecommerce
- Supply Chain
- Shipping
- Latin America
- 3PL
---
