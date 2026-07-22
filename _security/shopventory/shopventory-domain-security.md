---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shopventory.com
  spf: true
hosts:
- cert_expires: Aug 26 01:30:08 2026 GMT
  host: shopventory.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shopventory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shopventory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shopventory
provider_slug: shopventory
slug: shopventory-domain-security
source_filename: shopventory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shopventory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:30:08 2026 GMT\n  hsts: false\ndomains:\n- domain: shopventory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopventory/refs/heads/main/security/shopventory-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Inventory Management
- Point of Sale
- Retail
- eCommerce
- Reporting
- Small Business
- Techstars
---
