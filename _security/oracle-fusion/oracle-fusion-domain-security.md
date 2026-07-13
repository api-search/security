---
api_specs:
- filename: api-rest-api.html
  format: yaml
  label: Oracle Fusion ERP REST API
  slug: oracle-fusion-erp-rest-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/22r3/farfa/api-rest-api.html
- filename: api-rest-api.html
  format: yaml
  label: Oracle Fusion HCM REST API
  slug: oracle-fusion-hcm-rest-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/human-resources/22r3/farws/api-rest-api.html
- filename: api-rest-api.html
  format: yaml
  label: Oracle Fusion SCM REST API
  slug: oracle-fusion-scm-rest-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/supply-chain-management/22r3/fasrs/api-rest-api.html
- filename: rest-api.html
  format: yaml
  label: Oracle Fusion CX Sales and Fusion Service REST API
  slug: oracle-fusion-cx-sales-and-fusion-service-rest-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/cx-sales/rest-api.html
- filename: oracle-fusion-common-openapi.yml
  format: yaml
  label: Oracle Fusion Common Features REST API
  slug: oracle-fusion-common-features-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-fusion/refs/heads/main/openapi/oracle-fusion-common-openapi.yml
- filename: oracle-fusion-project-management-openapi.yml
  format: yaml
  label: Oracle Fusion Project Management REST API
  slug: oracle-fusion-project-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-fusion/refs/heads/main/openapi/oracle-fusion-project-management-openapi.yml
- filename: oracle-fusion-epm-openapi.yml
  format: yaml
  label: Oracle Fusion EPM REST API
  slug: oracle-fusion-epm-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-fusion/refs/heads/main/openapi/oracle-fusion-epm-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
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
name: Oracle Fusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Fusion Cloud Applications, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Fusion Cloud Applications
provider_slug: oracle-fusion
slug: oracle-fusion-domain-security
source_filename: oracle-fusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: www.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-fusion/refs/heads/main/security/oracle-fusion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- CX
- Enterprise
- EPM
- ERP
- HCM
- Project Management
- REST API
- SaaS
- SCM
---
