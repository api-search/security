---
api_specs:
- filename: api-procurement.html
  format: yaml
  label: Oracle Procurement REST API
  slug: oracle-procurement-rest-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/procurement/23d/fapra/api-procurement.html
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: cloud.oracle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Procurement Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Procurement, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Procurement
provider_slug: oracle-procurement
slug: oracle-procurement-domain-security
source_filename: oracle-procurement-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-procurement/refs/heads/main/security/oracle-procurement-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ERP
- Procurement
- Purchasing
- Spend Management
- Suppliers
---
