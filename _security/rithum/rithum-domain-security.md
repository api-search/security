---
api_specs:
- filename: dsco-platform-openapi.yml
  format: yaml
  label: Dsco Platform API
  slug: dsco-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/openapi/dsco-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rithum.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dsco.io
  spf: true
hosts:
- cert_expires: Aug 11 18:56:48 2026 GMT
  host: www.rithum.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: api.dsco.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rithum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rithum, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rithum
provider_slug: rithum
slug: rithum-domain-security
source_filename: rithum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rithum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 18:56:48 2026 GMT\n  hsts: false\n- host: api.dsco.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: rithum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dsco.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/security/rithum-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Commerce
- Dropship
- Marketplace
- Ecommerce
- Supply Chain
- Retail
---
