---
api_specs:
- filename: schema_retrieve
  format: yaml
  label: Authentik REST API
  slug: authentik-rest-api
  spec_type: OpenAPI
  url: https://api.goauthentik.io/#/Schema/schema_retrieve
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "infrastructure+caa@goauthentik.io"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuemail ";"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: goauthentik.io
  spf: true
hosts:
- cert_expires: Oct  6 04:10:40 2026 GMT
  host: goauthentik.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 21:48:53 2026 GMT
  host: api.goauthentik.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Authentik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Authentik, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Authentik
provider_slug: authentik
slug: authentik-domain-security
source_filename: authentik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goauthentik.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:10:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.goauthentik.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:48:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: goauthentik.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"infrastructure+caa@goauthentik.io\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuemail \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authentik/refs/heads/main/security/authentik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Authentication
- Authorization
- Identity Provider
- LDAP
- OAuth
- Open Source
- OpenID Connect
- SAML
- SCIM
- Self-Hosted
---
