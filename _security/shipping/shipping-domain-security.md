---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shipping.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freightos.com
  spf: true
hosts:
- host: www.shipping.com
  https: false
- cert_expires: Aug 26 14:59:27 2026 GMT
  host: fbx.freightos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 10:53:46 2026 GMT
  host: www.worldbank.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shipping Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shipping.com, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Shipping.com
provider_slug: shipping
slug: shipping-domain-security
source_filename: shipping-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shipping.com\n  https: false\n- host: fbx.freightos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 14:59:27 2026 GMT\n  hsts: false\n- host: www.worldbank.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 10:53:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shipping.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: freightos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipping/refs/heads/main/security/shipping-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shipping
- Freight
- Logistics
- Transportation
- Marketplace
- Rate Intelligence
- Ocean Freight
- Supply Chain
---
