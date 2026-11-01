---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: shopspring.ca
  spf: true
hosts:
- cert_expires: Dec 30 10:16:07 2026 GMT
  host: www.shopspring.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shopspring Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spring *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Spring *
provider_slug: shopspring-com
slug: shopspring-com-domain-security
source_filename: shopspring-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shopspring.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 10:16:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shopspring.ca\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/shopspring-com/security/shopspring-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- E-commerce
- Marketing
- SaaS
- Platform
---
