---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Authelia REST API
  slug: authelia-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/authelia/authelia/master/api/openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: authelia.com
  spf: true
hosts:
- cert_expires: Sep 12 01:23:53 2026 GMT
  host: www.authelia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Authelia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Authelia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Authelia
provider_slug: authelia
slug: authelia-domain-security
source_filename: authelia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.authelia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 01:23:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: authelia.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/security/authelia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Authentication
- Authorization
- LDAP
- MFA
- Open Source
- OpenID Connect
- Self-Hosted
- SSO
---
