---
api_specs:
- filename: elastic-path-commerce-apis.zip
  format: yaml
  label: Elastic Path Commerce Cloud API
  slug: commerce-cloud-api
  spec_type: OpenAPI
  url: https://developer.elasticpath.com/elastic-path-commerce-apis.zip
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elasticpath.com
  spf: true
hosts:
- cert_expires: Sep  6 15:00:28 2026 GMT
  host: www.elasticpath.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 06:12:41 2026 GMT
  host: developer.elasticpath.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 03:38:01 2026 GMT
  host: useast.api.elasticpath.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elastic Path Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elastic Path, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Elastic Path
provider_slug: elastic-path
slug: elastic-path-domain-security
source_filename: elastic-path-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elasticpath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:00:28 2026 GMT\n  hsts: null\n- host: developer.elasticpath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:12:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: useast.api.elasticpath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 03:38:01 2026 GMT\n  hsts: null\ndomains:\n- domain: elasticpath.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic-path/refs/heads/main/security/elastic-path-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Headless Commerce
- Composable Commerce
- eCommerce
- B2B
- Products
- Catalogs
- Orders
- Promotions
- Subscriptions
- Payments
---
