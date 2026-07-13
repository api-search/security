---
api_specs:
- filename: digicert-openapi.yml
  format: yaml
  label: DigiCert Services API
  slug: digicert-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digicert/refs/heads/main/openapi/digicert-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: digicert.com
  spf: true
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: false
  domain: digicert.eu
  spf: false
hosts:
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: www.digicert.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: dev.digicert.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 23:59:59 2026 GMT
  host: certcentral.digicert.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digicert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digicert, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Digicert
provider_slug: digicert
slug: digicert-domain-security
source_filename: digicert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digicert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.digicert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: certcentral.digicert.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: digicert.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: digicert.eu\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digicert/refs/heads/main/security/digicert-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Certificates
- Encryption
- PKI
- SSL
- TLS
---
