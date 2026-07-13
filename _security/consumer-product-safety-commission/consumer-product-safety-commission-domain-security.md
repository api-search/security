---
api_specs:
- filename: cpsc-recalls-openapi.yml
  format: yaml
  label: CPSC Recalls API
  slug: recalls
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consumer-product-safety-commission/refs/heads/main/openapi/cpsc-recalls-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cpsc.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: saferproducts.gov
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.cpsc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.saferproducts.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Consumer Product Safety Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Consumer Product Safety Commission, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Consumer Product Safety Commission
provider_slug: consumer-product-safety-commission
slug: consumer-product-safety-commission-domain-security
source_filename: consumer-product-safety-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cpsc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\n- host: www.saferproducts.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cpsc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: saferproducts.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consumer-product-safety-commission/refs/heads/main/security/consumer-product-safety-commission-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Consumer Protection
- Federal Government
- Hazards
- Open Data
- Product Safety
- Recalls
---
