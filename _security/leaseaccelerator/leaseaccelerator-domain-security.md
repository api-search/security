---
api_specs:
- filename: leaseaccelerator-api-openapi.yml
  format: yaml
  label: LeaseAccelerator API
  slug: leaseaccelerator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseaccelerator/refs/heads/main/openapi/leaseaccelerator-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: insightsoftware.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: leaseaccelerator.com
  spf: false
hosts:
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: insightsoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 15:13:53 2026 GMT
  host: docs-leaseaccelerator.insightsoftware.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: www.leaseaccelerator.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Leaseaccelerator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeaseAccelerator, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LeaseAccelerator
provider_slug: leaseaccelerator
slug: leaseaccelerator-domain-security
source_filename: leaseaccelerator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insightsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs-leaseaccelerator.insightsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 15:13:53 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: www.leaseaccelerator.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: insightsoftware.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: leaseaccelerator.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaseaccelerator/refs/heads/main/security/leaseaccelerator-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Lease Accounting
- Lease Administration
- Financial Reporting
- Enterprise Software
- Accounting
- Real Estate
- Asset Management
- ERP Integration
- Compliance
---
