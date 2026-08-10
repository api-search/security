---
api_specs:
- filename: bond-pet-foods-wc-store-v1-api-openapi.yml
  format: yaml
  label: Bond Pet Foods Wc/store/v1 API
  slug: bond-pet-foods-wc-store-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond-pet-foods/refs/heads/main/openapi/bond-pet-foods-wc-store-v1-api-openapi.yml
- filename: bond-pet-foods-wp-v2-api-openapi.yml
  format: yaml
  label: Bond Pet Foods Wp/v2 API
  slug: bond-pet-foods-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond-pet-foods/refs/heads/main/openapi/bond-pet-foods-wp-v2-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bondpets.com
  spf: true
hosts:
- cert_expires: Oct 26 11:34:44 2026 GMT
  host: www.bondpets.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bond Pet Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bond Pet Foods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bond Pet Foods
provider_slug: bond-pet-foods
slug: bond-pet-foods-domain-security
source_filename: bond-pet-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bondpets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 11:34:44 2026 GMT\n  hsts: false\ndomains:\n- domain: bondpets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bond-pet-foods/refs/heads/main/security/bond-pet-foods-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pet Food
- Alternative Protein
- Precision Fermentation
- Food Technology
- Biotechnology
- Animal Nutrition
- Sustainability
- E-Commerce
- WooCommerce
- WordPress
---
