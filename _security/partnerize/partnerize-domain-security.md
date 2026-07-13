---
api_specs:
- filename: partnerize-brands-api-openapi.yml
  format: yaml
  label: Partnerize Brands API
  slug: brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/partnerize/refs/heads/main/openapi/partnerize-brands-api-openapi.yml
- filename: partnerize-partners-api-openapi.yml
  format: yaml
  label: Partnerize Partners API
  slug: partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/partnerize/refs/heads/main/openapi/partnerize-partners-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: partnerize.com
  spf: true
hosts:
- cert_expires: Aug 18 01:34:08 2026 GMT
  host: partnerize.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api-docs.partnerize.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.partnerize.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Partnerize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Partnerize, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Partnerize
provider_slug: partnerize
slug: partnerize-domain-security
source_filename: partnerize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: partnerize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 01:34:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.partnerize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\n- host: api.partnerize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: partnerize.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/partnerize/refs/heads/main/security/partnerize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Affiliate Marketing
- Partner Marketing
- Partnerships
- Performance Marketing
- Commissions
- Tracking
- Analytics
---
