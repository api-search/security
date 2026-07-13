---
api_specs:
- filename: isg-rest-api.yml
  format: yaml
  label: Oracle EBS Integrated SOA Gateway REST API
  slug: oracle-ebs-integrated-soa-gateway-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/isg-rest-api.yml
- filename: financial-services-api.yml
  format: yaml
  label: Oracle EBS Financial Services API
  slug: oracle-ebs-financial-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/financial-services-api.yml
- filename: supply-chain-api.yml
  format: yaml
  label: Oracle EBS Supply Chain Management API
  slug: oracle-ebs-supply-chain-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/supply-chain-api.yml
- filename: human-resources-api.yml
  format: yaml
  label: Oracle EBS Human Resources API
  slug: oracle-ebs-human-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/human-resources-api.yml
- filename: manufacturing-api.yml
  format: yaml
  label: Oracle EBS Manufacturing API
  slug: oracle-ebs-manufacturing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/manufacturing-api.yml
- filename: ecommerce-gateway-api.yml
  format: yaml
  label: Oracle EBS e-Commerce Gateway API
  slug: oracle-ebs-e-commerce-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/openapi/ecommerce-gateway-api.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: developer.oracle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle E Business Suite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle E-Business Suite, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
slug: oracle-e-business-suite-domain-security
source_filename: oracle-e-business-suite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/security/oracle-e-business-suite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
---
