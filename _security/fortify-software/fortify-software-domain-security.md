---
api_specs:
- filename: fortify-software-fod-openapi.json
  format: json
  label: Fortify on Demand REST API (v3)
  slug: fortify-on-demand-rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortify-software/refs/heads/main/openapi/fortify-software-fod-openapi.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: opentext.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fortify.com
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: www.opentext.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: api.ams.fortify.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fortify Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortify Software, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fortify Software
provider_slug: fortify-software
slug: fortify-software-domain-security
source_filename: fortify-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opentext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\n- host: api.ams.fortify.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: opentext.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fortify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortify-software/refs/heads/main/security/fortify-software-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Application Security
- AppSec
- SAST
- DAST
- Vulnerability Management
- DevSecOps
- Software Composition Analysis
- API Security
---
