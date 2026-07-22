---
api_specs:
- filename: refurbed-merchant-api-openapi.json
  format: json
  label: Refurbed Merchant API
  slug: refurbed-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-merchant-api-openapi.json
- filename: refurbed-affiliate-api-openapi.json
  format: json
  label: Refurbed Affiliate Partner API
  slug: refurbed-affiliate-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/openapi/refurbed-affiliate-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: refurbed.com
  spf: true
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gitlab.com
  spf: true
hosts:
- cert_expires: Oct 10 20:04:42 2026 GMT
  host: www.refurbed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: gitlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 00:39:40 2026 GMT
  host: api.refurbed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Refurbed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Refurbed, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Refurbed
provider_slug: refurbed
slug: refurbed-domain-security
source_filename: refurbed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.refurbed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 20:04:42 2026 GMT\n  hsts: null\n- host: gitlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.refurbed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 00:39:40 2026 GMT\n  hsts: null\ndomains:\n- domain: refurbed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gitlab.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refurbed/refs/heads/main/security/refurbed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- E-Commerce
- Refurbished Electronics
- Sustainability
- Circular Economy
- Retail
- Merchant API
- Affiliate
- gRPC
---
