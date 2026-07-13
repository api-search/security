---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: prestashop.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: prestashop-project.org
  spf: false
hosts:
- cert_expires: Aug  5 08:30:43 2026 GMT
  host: www.prestashop.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 14:15:08 2026 GMT
  host: devdocs.prestashop-project.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prestashop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PrestaShop, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: PrestaShop
provider_slug: prestashop
slug: prestashop-domain-security
source_filename: prestashop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prestashop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 08:30:43 2026 GMT\n  hsts: false\n- host: devdocs.prestashop-project.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 14:15:08 2026 GMT\n  hsts: false\ndomains:\n- domain: prestashop.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: prestashop-project.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prestashop/refs/heads/main/security/prestashop-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- E-Commerce
- Open Source
- Products
- Orders
- Customers
- Inventory
- Catalog
- Carriers
- Stock
- Tax
---
