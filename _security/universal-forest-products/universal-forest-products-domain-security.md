---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ufpi.com
  spf: true
hosts:
- cert_expires: Aug 24 05:47:26 2026 GMT
  host: ufpi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Universal Forest Products Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universal Forest Products, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Universal Forest Products
provider_slug: universal-forest-products
slug: universal-forest-products-domain-security
source_filename: universal-forest-products-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ufpi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 05:47:26 2026 GMT\n  hsts: false\ndomains:\n- domain: ufpi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universal-forest-products/refs/heads/main/security/universal-forest-products-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Manufacturing
- Construction
- Wood Products
- Supply Chain
- Building Materials
- Fortune 1000
---
