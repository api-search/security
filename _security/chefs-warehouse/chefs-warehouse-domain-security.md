---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chefswarehouse.com
  spf: true
hosts:
- cert_expires: Aug 14 17:54:01 2026 GMT
  host: www.chefswarehouse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chefs Warehouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chefs'' Warehouse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chefs' Warehouse
provider_slug: chefs-warehouse
slug: chefs-warehouse-domain-security
source_filename: chefs-warehouse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chefswarehouse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 17:54:01 2026 GMT\n  hsts: false\ndomains:\n- domain: chefswarehouse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chefs-warehouse/refs/heads/main/security/chefs-warehouse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Food Distribution
- Specialty Food
- Foodservice
- Wholesale
- Restaurants
- Ecommerce
- B2B Commerce
- Supply Chain
---
