---
api_specs:
- filename: pingone-platform-api
  format: yaml
  label: PingOne Platform API
  slug: platform-api
  spec_type: Postman
  url: https://www.postman.com/ping-identity/pingone/collection/xu0baxr/pingone-platform-api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pingidentity.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pingone.com
  spf: true
hosts:
- cert_expires: Sep  4 20:14:53 2026 GMT
  host: www.pingidentity.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: apidocs.pingidentity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: api.pingone.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pingone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PingOne, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PingOne
provider_slug: pingone
slug: pingone-domain-security
source_filename: pingone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pingidentity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:14:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: apidocs.pingidentity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\n- host: api.pingone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pingidentity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pingone.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pingone/refs/heads/main/security/pingone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity
- Authentication
- Authorization
- Single Sign-On
- Multi-Factor Authentication
- IAM
- CIAM
---
