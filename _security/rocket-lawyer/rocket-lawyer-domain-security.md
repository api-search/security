---
api_specs:
- filename: rocket-lawyer-authentication-api-openapi.yml
  format: yaml
  label: Rocket Lawyer Authentication API
  slug: rocket-lawyer-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-lawyer/refs/heads/main/openapi/rocket-lawyer-authentication-api-openapi.yml
- filename: rocket-lawyer-rocketdocument-api-openapi.yml
  format: yaml
  label: Rocket Lawyer RocketDocument v2 API
  slug: rocket-lawyer-rocketdocument-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-lawyer/refs/heads/main/openapi/rocket-lawyer-rocketdocument-api-openapi.yml
- filename: rocket-lawyer-rocketsign-binders-api-openapi.yml
  format: yaml
  label: Rocket Lawyer RocketSign and Binders API
  slug: rocket-lawyer-rocketsign-binders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-lawyer/refs/heads/main/openapi/rocket-lawyer-rocketsign-binders-api-openapi.yml
- filename: rocket-lawyer-events-api-openapi.yml
  format: yaml
  label: Rocket Lawyer Events API
  slug: rocket-lawyer-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-lawyer/refs/heads/main/openapi/rocket-lawyer-events-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rocketlawyer.com
  spf: true
hosts:
- cert_expires: Apr  4 22:07:28 2027 GMT
  host: www.rocketlawyer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 16:40:13 2026 GMT
  host: developer.rocketlawyer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 20:08:33 2026 GMT
  host: api.rocketlawyer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rocket Lawyer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rocket Lawyer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Rocket Lawyer
provider_slug: rocket-lawyer
slug: rocket-lawyer-domain-security
source_filename: rocket-lawyer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rocketlawyer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  4 22:07:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.rocketlawyer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:40:13 2026 GMT\n  hsts: null\n- host: api.rocketlawyer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 20:08:33 2026 GMT\n  hsts: null\ndomains:\n- domain: rocketlawyer.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocket-lawyer/refs/heads/main/security/rocket-lawyer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Legal
- Legal Technology
- LegalTech
- Legal Documents
- Electronic Signature
- eSignature
- Document Creation
- Document Management
- Business Formation
- LLC Formation
- Registered Agent
- Trademark
- Wills
- Estate Planning
- Attorney Network
- Small Business
- Membership
- Embedded UX
- Partner API
- Apigee
- OpenAPI
---
