---
api_specs:
- filename: v3
  format: yaml
  label: Fortify on Demand API
  slug: fortify-on-demand-api
  spec_type: OpenAPI
  url: https://api.ams.fortify.com/swagger/docs/v3
- filename: fortify-software-security-center-openapi.yml
  format: yaml
  label: Fortify Software Security Center API
  slug: fortify-software-security-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortify/refs/heads/main/openapi/fortify-software-security-center-openapi.yml
- filename: fortify-scancentral-dast-openapi.yml
  format: yaml
  label: Fortify ScanCentral DAST API
  slug: fortify-scancentral-dast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortify/refs/heads/main/openapi/fortify-scancentral-dast-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fortify.com
  spf: true
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: opentext.com
  spf: true
hosts:
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: ams.fortify.com
  hsts: null
  https: true
  tls_version: TLSv1.2
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
name: Fortify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortify, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fortify
provider_slug: fortify
slug: fortify-domain-security
source_filename: fortify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ams.fortify.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: null\n- host: www.opentext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\n- host: api.ams.fortify.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fortify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: opentext.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortify/refs/heads/main/security/fortify-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Application Security
- DAST
- DevSecOps
- SAST
- SCA
- Security Testing
- Vulnerability Scanning
---
