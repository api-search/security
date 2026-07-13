---
api_specs:
- filename: index.html
  format: yaml
  label: Extensis Portfolio REST API
  slug: extensis-portfolio-rest-api
  spec_type: OpenAPI
  url: https://doc.extensis.com/api/portfolio/rest/index.html
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: extensis.com
  spf: true
hosts:
- cert_expires: Oct  7 16:43:36 2026 GMT
  host: www.extensis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: doc.extensis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: portfolio.extensis.com
  https: false
kind: domain-security
layout: security
method: probed
name: Extensis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Extensis, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Extensis
provider_slug: extensis
slug: extensis-domain-security
source_filename: extensis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.extensis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:43:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc.extensis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\n- host: portfolio.extensis.com\n  https: false\ndomains:\n- domain: extensis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extensis/refs/heads/main/security/extensis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Asset Management
- Font Management
- Creative Assets
- Font Licensing
- Design Workflows
- DAM
---
