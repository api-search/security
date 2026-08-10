---
api_specs:
- filename: eruditus-executive-education-leads-api-openapi.yml
  format: yaml
  label: Eruditus Leads API
  slug: eruditus-executive-education-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eruditus-executive-education/refs/heads/main/openapi/eruditus-executive-education-leads-api-openapi.yml
- filename: eruditus-executive-education-programs-api-openapi.yml
  format: yaml
  label: Eruditus Programs API
  slug: eruditus-executive-education-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eruditus-executive-education/refs/heads/main/openapi/eruditus-executive-education-programs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eruditus.com
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emeritus.org
  spf: true
hosts:
- cert_expires: Oct 24 04:28:01 2026 GMT
  host: eruditus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 04:28:00 2026 GMT
  host: emeritus.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 08:16:46 2026 GMT
  host: admissions.emeritus.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eruditus Executive Education Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eruditus, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eruditus
provider_slug: eruditus-executive-education
slug: eruditus-executive-education-domain-security
source_filename: eruditus-executive-education-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eruditus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 04:28:01 2026 GMT\n  hsts: null\n- host: emeritus.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 04:28:00 2026 GMT\n  hsts: null\n- host: admissions.emeritus.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:16:46 2026 GMT\n  hsts: null\ndomains:\n- domain: eruditus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: emeritus.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nnotes:\n- host: admissions.emeritus.org\n  observed: 'strict-transport-security:\
  \ max-age=631138519'\n  method: manual probe of GET /api/v1/programs_api/programs, 2026-08-04\n  note: The API endpoints do return HSTS even though the automated HEAD probe of the host root recorded none.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eruditus-executive-education/refs/heads/main/security/eruditus-executive-education-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- Online Learning
- Executive Education
- EdTech
- Higher Education
- Leads
- Enrollment
- Programs
- Singapore
---
