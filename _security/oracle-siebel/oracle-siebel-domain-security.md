---
api_specs:
- filename: oracle-siebel-accounts-api-openapi.yml
  format: yaml
  label: Oracle Siebel Accounts API
  slug: oracle-siebel-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-accounts-api-openapi.yml
- filename: oracle-siebel-activities-api-openapi.yml
  format: yaml
  label: Oracle Siebel Activities API
  slug: oracle-siebel-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-activities-api-openapi.yml
- filename: oracle-siebel-business-services-api-openapi.yml
  format: yaml
  label: Oracle Siebel Business Services API
  slug: oracle-siebel-business-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-business-services-api-openapi.yml
- filename: oracle-siebel-contacts-api-openapi.yml
  format: yaml
  label: Oracle Siebel Contacts API
  slug: oracle-siebel-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-contacts-api-openapi.yml
- filename: oracle-siebel-metadata-api-openapi.yml
  format: yaml
  label: Oracle Siebel Metadata API
  slug: oracle-siebel-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-metadata-api-openapi.yml
- filename: oracle-siebel-opportunities-api-openapi.yml
  format: yaml
  label: Oracle Siebel Opportunities API
  slug: oracle-siebel-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-opportunities-api-openapi.yml
- filename: oracle-siebel-orders-api-openapi.yml
  format: yaml
  label: Oracle Siebel Orders API
  slug: oracle-siebel-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-orders-api-openapi.yml
- filename: oracle-siebel-products-api-openapi.yml
  format: yaml
  label: Oracle Siebel Products API
  slug: oracle-siebel-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-products-api-openapi.yml
- filename: oracle-siebel-repository-api-openapi.yml
  format: yaml
  label: Oracle Siebel Repository API
  slug: oracle-siebel-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-repository-api-openapi.yml
- filename: oracle-siebel-service-requests-api-openapi.yml
  format: yaml
  label: Oracle Siebel Service Requests API
  slug: oracle-siebel-service-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-service-requests-api-openapi.yml
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
name: Oracle Siebel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Siebel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Siebel
provider_slug: oracle-siebel
slug: oracle-siebel-domain-security
source_filename: oracle-siebel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: www.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/security/oracle-siebel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Customer Management
- Enterprise Software
- Marketing Automation
- Oracle
- Sales Automation
- Service Automation
---
