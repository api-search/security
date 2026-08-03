---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aptera.us
  spf: true
hosts:
- cert_expires: Sep  2 18:11:29 2026 GMT
  host: aptera.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 11:10:02 2026 GMT
  host: shop.aptera.us
  hsts: true
  hsts_max_age: 7889238
  https: true
  note: Shopify-hosted merchandise storefront (powered-by Shopify)
  tls_version: TLSv1.3
- cert_expires: Sep  1 20:36:31 2026 GMT
  host: ir.aptera.us
  hsts: false
  https: true
  note: investor relations host; returns no HSTS header and did not complete an HTTP response to the probe user-agent
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aptera Motors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aptera Motors, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aptera Motors
provider_slug: aptera-motors
slug: aptera-motors-domain-security
source_filename: aptera-motors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aptera.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 18:11:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: shop.aptera.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 11:10:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n  note: Shopify-hosted merchandise storefront (powered-by Shopify)\n- host: ir.aptera.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 20:36:31 2026 GMT\n  hsts: false\n  note: investor relations host; returns no HSTS header and did not complete an HTTP\n    response to the probe user-agent\ndomains:\n- domain: aptera.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aptera-motors/refs/heads/main/security/aptera-motors-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Electric Vehicles
- Solar
- Manufacturing
- Clean Energy
- Transportation
- Consumer Products
- Mobility
---
