---
api_specs:
- filename: delphix-continuous-data-openapi.yml
  format: yaml
  label: Delphix DCT Continuous Data API
  slug: delphix-dct-continuous-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delphix/refs/heads/main/openapi/delphix-continuous-data-openapi.yml
- filename: delphix-continuous-compliance-openapi.yml
  format: yaml
  label: Delphix DCT Continuous Compliance API
  slug: delphix-dct-continuous-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delphix/refs/heads/main/openapi/delphix-continuous-compliance-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@perforce.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: perforce.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: delphix.com
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: www.perforce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 08:12:19 2026 GMT
  host: help-api.delphix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Delphix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delphix, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Delphix
provider_slug: delphix
slug: delphix-domain-security
source_filename: delphix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.perforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help-api.delphix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 08:12:19 2026 GMT\n  hsts: false\ndomains:\n- domain: perforce.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@perforce.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: delphix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delphix/refs/heads/main/security/delphix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Management
- Test Data Management
- Data Virtualization
- Data Masking
- Data Compliance
- Database
- DevOps
- Synthetic Data
- Data Control Tower
---
