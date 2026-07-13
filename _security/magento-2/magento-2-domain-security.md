---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: business.adobe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: developer.adobe.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Magento 2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magento 2 (Adobe Commerce), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Magento 2 (Adobe Commerce)
provider_slug: magento-2
slug: magento-2-domain-security
source_filename: magento-2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: business.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magento-2/refs/heads/main/security/magento-2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ecommerce
- Commerce
- Online Store
- Catalog Management
- Order Management
- GraphQL
- REST
- SOAP
---
