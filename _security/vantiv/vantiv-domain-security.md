---
api_specs:
- filename: vantiv-cnp-openapi.yml
  format: yaml
  label: Vantiv CNP API
  slug: cnp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-cnp-openapi.yml
- filename: vantiv-express-openapi.yml
  format: yaml
  label: Vantiv Express API
  slug: express-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-express-openapi.yml
- filename: vantiv-chargeback-openapi.yml
  format: yaml
  label: Vantiv Chargeback API
  slug: chargeback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/openapi/vantiv-chargeback-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vantiv.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vantivprelive.com
  spf: true
hosts:
- host: developer.vantiv.com
  https: false
- host: www.vantiv.com
  https: false
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: payments.vantivprelive.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vantiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vantiv, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vantiv
provider_slug: vantiv
slug: vantiv-domain-security
source_filename: vantiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.vantiv.com\n  https: false\n- host: www.vantiv.com\n  https: false\n- host: payments.vantivprelive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: vantiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: vantivprelive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vantiv/refs/heads/main/security/vantiv-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Payment Processing
- eCommerce
- Finance
- FinTech
- Fortune 1000
---
