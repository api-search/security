---
api_specs:
- filename: icecat-biz-openapi-generated.yml
  format: yaml
  label: Icecat API
  slug: icecat-biz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/icecat-biz/openapi/_ae-authored/icecat-biz-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: icecat.biz
  spf: true
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: icecat.biz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Icecat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Icecat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Icecat
provider_slug: icecat-biz
slug: icecat-biz-domain-security
source_filename: icecat-biz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: icecat.biz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: icecat.biz\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/icecat-biz/security/icecat-biz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Product Catalog
- Data Feed
- Multilingual
---
