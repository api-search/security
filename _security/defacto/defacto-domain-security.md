---
api_specs:
- filename: defacto-openapi-original.json
  format: json
  label: Defacto API
  slug: defacto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-openapi-original.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@getdefacto.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: getdefacto.com
  spf: true
hosts:
- cert_expires: Sep 27 17:32:20 2026 GMT
  host: www.getdefacto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 14:33:02 2026 GMT
  host: api.getdefacto.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: api-sandbox.getdefacto.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Defacto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defacto, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Defacto
provider_slug: defacto
slug: defacto-domain-security
source_filename: defacto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getdefacto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:32:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getdefacto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 14:33:02 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api-sandbox.getdefacto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: getdefacto.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@getdefacto.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/security/defacto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Embedded Finance
- Lending
- Working Capital
- Invoice Financing
- Credit
- B2B Payments
- SMB
- France
- Europe
---
