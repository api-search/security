---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airproducts.com
  spf: true
hosts:
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: www.airproducts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 20:36:31 2026 GMT
  host: investors.airproducts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Air Products And Chemicals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Air Products and Chemicals, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Air Products and Chemicals
provider_slug: air-products-and-chemicals
slug: air-products-and-chemicals-domain-security
source_filename: air-products-and-chemicals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airproducts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\n- host: investors.airproducts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 20:36:31 2026 GMT\n  hsts: null\ndomains:\n- domain: airproducts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/air-products-and-chemicals/refs/heads/main/security/air-products-and-chemicals-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Industrial Gases
- Chemicals
- Energy
- Manufacturing
- Hydrogen
- Enterprise
---
