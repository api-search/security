---
api_specs:
- filename: bloomberg-emsx-trading-openapi.yml
  format: yaml
  label: Bloomberg EMSX Trading API
  slug: bloomberg-emsx-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-emsx/refs/heads/main/openapi/bloomberg-emsx-trading-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:reportvuln@bloomberg.net"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bloomberg.com
  spf: true
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue " amazontrust.com"
  - 0 issue "comodoca.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: www.bloomberg.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: emsx-api-doc.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 21 23:59:59 2027 GMT
  host: api.bloomberg.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloomberg Emsx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomberg EMSX, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bloomberg EMSX
provider_slug: bloomberg-emsx
slug: bloomberg-emsx-domain-security
source_filename: bloomberg-emsx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bloomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\n- host: emsx-api-doc.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bloomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bloomberg.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:reportvuln@bloomberg.net\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"\
  ssl.com\"\n  - 0 issue \" amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-emsx/refs/heads/main/security/bloomberg-emsx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bloomberg
- Execution Management
- Financial Services
- Order Management
- Trading
---
