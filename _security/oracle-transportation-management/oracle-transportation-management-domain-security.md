---
api_specs:
- filename: oracle-otm-business-objects-openapi.yml
  format: yaml
  label: Oracle Transportation Management Business Object Resources REST API
  slug: oracle-transportation-management-business-object-resources-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-transportation-management/refs/heads/main/openapi/oracle-otm-business-objects-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.oracle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Transportation Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Transportation Management, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Transportation Management
provider_slug: oracle-transportation-management
slug: oracle-transportation-management-domain-security
source_filename: oracle-transportation-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: www.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-transportation-management/refs/heads/main/security/oracle-transportation-management-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Transportation
- Freight
- Supply Chain
- Shipping
- Global Trade
- Oracle
---
