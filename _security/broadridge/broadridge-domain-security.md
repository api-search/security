---
api_specs:
- filename: broadridge-wealth-openapi.yml
  format: yaml
  label: Broadridge Wealth Management API
  slug: broadridge-wealth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadridge/refs/heads/main/openapi/broadridge-wealth-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:bsg.hostmaster@broadridge.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: broadridge.com
  spf: true
- caa:
  - 0 issue "entrust.net"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:bsg.hostmaster@broadridge.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fundslibrary.net
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.broadridge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: dataapi-web.fundslibrary.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Broadridge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for broadridge, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: broadridge
provider_slug: broadridge
slug: broadridge-domain-security
source_filename: broadridge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.broadridge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dataapi-web.fundslibrary.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: broadridge.com\n  dnssec: false\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:bsg.hostmaster@broadridge.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fundslibrary.net\n  dnssec: false\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:bsg.hostmaster@broadridge.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/broadridge/refs/heads/main/security/broadridge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 1000
---
