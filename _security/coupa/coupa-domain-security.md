---
api_specs:
- filename: coupa-invoices-api-openapi.yml
  format: yaml
  label: Coupa Invoices API
  slug: coupa-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupa/openapi/coupa-invoices-api-openapi.yml
- filename: coupa-purchase-orders-api-openapi.yml
  format: yaml
  label: Coupa Purchase Orders API
  slug: coupa-purchase-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupa/openapi/coupa-purchase-orders-api-openapi.yml
- filename: coupa-requisitions-api-openapi.yml
  format: yaml
  label: Coupa Requisitions API
  slug: coupa-requisitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupa/openapi/coupa-requisitions-api-openapi.yml
- filename: coupa-suppliers-api-openapi.yml
  format: yaml
  label: Coupa Suppliers API
  slug: coupa-suppliers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupa/openapi/coupa-suppliers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coupa.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: coupahost.com
  spf: true
hosts:
- cert_expires: Jan 27 01:52:26 2027 GMT
  host: coupa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: May 13 23:59:59 2027 GMT
  host: compass.coupa.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
- host: instance.coupahost.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Coupa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coupa, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coupa
provider_slug: coupa
slug: coupa-domain-security
source_filename: coupa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coupa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 01:52:26 2027 GMT\n  hsts: null\n- host: compass.coupa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: instance.coupahost.com\n  https: false\ndomains:\n- domain: coupa.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: coupahost.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/coupa/security/coupa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- BSM
- Business Spend Management
- Cloud Platform
- Enterprise
- Financial Management
- Invoicing
- Procurement
- Supply Chain
---
