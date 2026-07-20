---
api_specs:
- filename: postman
  format: yaml
  label: Forescout Web API (Open Integration Module)
  slug: forescout-web-api-open-integration-module
  spec_type: Postman
  url: https://github.com/Forescout/examples/tree/master/web-api/postman
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: forescout.com
  spf: true
hosts:
- cert_expires: Sep  6 22:31:19 2026 GMT
  host: www.forescout.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forescout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forescout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Forescout
provider_slug: forescout
slug: forescout-domain-security
source_filename: forescout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.forescout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:31:19 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: forescout.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forescout/refs/heads/main/security/forescout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Network Security
- Device Visibility
- Asset Inventory
- OT Security
- IoT Security
- Vulnerability Management
- Zero Trust
- REST API
---
