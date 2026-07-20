---
api_specs:
- filename: channable-order-connection-openapi.json
  format: json
  label: Channable Order Connection API
  slug: channable-order-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channable/refs/heads/main/openapi/channable-order-connection-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: channable.com
  spf: true
hosts:
- cert_expires: Oct 14 16:21:36 2026 GMT
  host: www.channable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 16:35:19 2026 GMT
  host: docs.channable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 13:52:26 2026 GMT
  host: api.channable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Channable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Channable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Channable
provider_slug: channable
slug: channable-domain-security
source_filename: channable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.channable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:21:36 2026 GMT\n  hsts: null\n- host: docs.channable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 16:35:19 2026 GMT\n  hsts: false\n- host: api.channable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 13:52:26 2026 GMT\n  hsts: false\ndomains:\n- domain: channable.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channable/refs/heads/main/security/channable-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Applicative Saas
- Feed Management
- Marketplaces
- E-commerce
- Product Data
- Order Management
- Advertising
- PPC
- Retail
---
