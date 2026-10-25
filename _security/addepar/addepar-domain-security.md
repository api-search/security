---
api_specs:
- filename: addepar-openapi-generated.yml
  format: yaml
  label: Addepar API
  slug: addepar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addepar/refs/heads/main/openapi/_ae-authored/addepar-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "Digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: addepar.com
  spf: true
hosts:
- cert_expires: Nov 29 05:13:48 2026 GMT
  host: addepar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 11:16:02 2026 GMT
  host: developers.addepar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.addepar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Addepar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Addepar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Addepar
provider_slug: addepar
slug: addepar-domain-security
source_filename: addepar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: addepar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 05:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.addepar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 11:16:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.addepar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: addepar.com\n  dnssec: false\n  caa:\n  - 0 issue \"Digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/addepar/refs/heads/main/security/addepar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Wealth Management
- Portfolio Management
- Investment Management
- Financial Data
- JSON:API
- REST
---
