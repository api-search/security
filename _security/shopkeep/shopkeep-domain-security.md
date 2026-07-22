---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "geotrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopkeep.com
  spf: true
hosts:
- cert_expires: Sep  4 08:04:43 2026 GMT
  host: www.shopkeep.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shopkeep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shopkeep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shopkeep
provider_slug: shopkeep
slug: shopkeep-domain-security
source_filename: shopkeep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shopkeep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 08:04:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shopkeep.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopkeep/refs/heads/main/security/shopkeep-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Point of Sale
- Retail
- Payments
- Small Business
- POS
- iPad
- Lightspeed
---
