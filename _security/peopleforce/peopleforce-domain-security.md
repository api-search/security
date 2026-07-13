---
api_specs:
- filename: peopleforce-openapi.yml
  format: yaml
  label: PeopleForce API
  slug: peopleforce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopleforce/refs/heads/main/openapi/peopleforce-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: peopleforce.io
  spf: true
hosts:
- cert_expires: Sep 22 10:10:07 2026 GMT
  host: developer.peopleforce.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 20:58:21 2026 GMT
  host: app.peopleforce.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peopleforce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PeopleForce, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PeopleForce
provider_slug: peopleforce
slug: peopleforce-domain-security
source_filename: peopleforce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.peopleforce.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:10:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.peopleforce.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 20:58:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: peopleforce.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peopleforce/refs/heads/main/security/peopleforce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- Human Resources
- Recruitment
- Employees
---
