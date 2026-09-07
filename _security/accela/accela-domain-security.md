---
api_specs:
- filename: accela-records-openapi.yml
  format: yaml
  label: Accela Construct API (V4)
  slug: accela-construct-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accela/refs/heads/main/openapi/accela-records-openapi.yml
- filename: accela-authentication-openapi.yml
  format: yaml
  label: Accela Authentication API (OAuth 2.0)
  slug: accela-authentication-api-oauth-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accela/refs/heads/main/openapi/accela-authentication-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: accela.com
  spf: true
hosts:
- cert_expires: Oct 26 02:08:18 2026 GMT
  host: www.accela.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 18:24:37 2027 GMT
  host: developer.accela.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 18:24:37 2027 GMT
  host: apis.accela.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Accela Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accela, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Accela
provider_slug: accela
slug: accela-domain-security
source_filename: accela-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accela.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 02:08:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: developer.accela.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 18:24:37 2027 GMT\n  hsts: false\n- host: apis.accela.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 18:24:37 2027 GMT\n  hsts: false\ndomains:\n- domain: accela.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accela/refs/heads/main/security/accela-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- GovTech
- Government
- Permitting
- Licensing
- Code Enforcement
- Inspections
- Asset Management
- Citizen Engagement
- Land Management
- Civic Platform
- Public Sector
- SaaS
---
