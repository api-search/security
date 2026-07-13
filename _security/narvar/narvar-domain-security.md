---
api_specs:
- filename: narvar-order-openapi.yml
  format: yaml
  label: Narvar Order API
  slug: narvar-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narvar/refs/heads/main/openapi/narvar-order-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "Digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:info@narvar.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: narvar.com
  spf: true
hosts:
- cert_expires: Oct  7 15:42:19 2026 GMT
  host: corp.narvar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:41:49 2026 GMT
  host: support.narvar.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 13 23:59:59 2026 GMT
  host: api.narvar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Narvar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Narvar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Narvar
provider_slug: narvar
slug: narvar-domain-security
source_filename: narvar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corp.narvar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:42:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.narvar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:41:49 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.narvar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: narvar.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"Digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:info@narvar.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/narvar/refs/heads/main/security/narvar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Post-Purchase
- Order Tracking
- Delivery Notifications
- Returns
- Exchanges
- Ecommerce
- Shipments
- Customer Experience
---
