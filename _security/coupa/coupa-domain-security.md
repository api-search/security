---
api_specs:
- filename: api_docs
  format: yaml
  label: Coupa Core API
  slug: coupa-core-api
  spec_type: OpenAPI
  url: https://compass.coupa.com/en-us/api_docs
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
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
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: compass.coupa.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
- host: instance.coupahost.com
  https: false
- host: instance.cso.coupahost.com
  https: false
kind: domain-security
layout: security
method: probed
name: Coupa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coupa, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coupa
provider_slug: coupa
slug: coupa-domain-security
source_filename: coupa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compass.coupa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: instance.coupahost.com\n  https: false\n- host: instance.cso.coupahost.com\n  https: false\ndomains:\n- domain: coupa.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: coupahost.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coupa/refs/heads/main/security/coupa-domain-security.yml
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
