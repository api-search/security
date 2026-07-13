---
api_specs:
- filename: cmic-construction-erp-openapi.yml
  format: yaml
  label: CMiC Construction ERP API
  slug: cmic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cmic/refs/heads/main/openapi/cmic-construction-erp-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issuewild "godaddy.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cmicglobal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cmic.ca
  spf: true
hosts:
- cert_expires: Sep 30 04:28:43 2026 GMT
  host: cmicglobal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 10:18:05 2026 GMT
  host: developers.cmicglobal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.cmic.ca
  https: false
kind: domain-security
layout: security
method: probed
name: Cmic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CMiC, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CMiC
provider_slug: cmic
slug: cmic-domain-security
source_filename: cmic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cmicglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:28:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.cmicglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 10:18:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cmic.ca\n  https: false\ndomains:\n- domain: cmicglobal.com\n  dnssec: true\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cmic.ca\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cmic/refs/heads/main/security/cmic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Construction
- ERP
- Finance
- Project Management
---
