---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Oracle Cloud Infrastructure (OCI) REST API
  slug: oracle-cloud-infrastructure-oci-rest-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en-us/iaas/api/#/en/iaas/latest/
- filename: openapi.yaml
  format: yaml
  label: Oracle Autonomous Database API
  slug: oracle-autonomous-database-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en-us/iaas/api/#/en/database/latest/
- filename: api-integration-cloud.html
  format: yaml
  label: Oracle Integration Cloud API
  slug: oracle-integration-cloud-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/paas/integration-cloud/rest-api/api-integration-cloud.html
- filename: api-rest.html
  format: yaml
  label: Oracle Analytics Cloud API
  slug: oracle-analytics-cloud-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/paas/analytics-cloud/acapi/api-rest.html
- filename: openapi.yaml
  format: yaml
  label: Oracle Cloud Infrastructure Data Science API
  slug: oracle-cloud-infrastructure-data-science-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en-us/iaas/api/#/en/data-science/latest/
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
- caa:
  - 0 issue "digicert.com"
  - 0 issue "symantec.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oraclecloud.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: integration.ocp.oraclecloud.com
  https: false
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: www.oraclecloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Platforms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Platforms, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Platforms
provider_slug: oracle-platforms
slug: oracle-platforms-domain-security
source_filename: oracle-platforms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: integration.ocp.oraclecloud.com\n  https: false\n- host: www.oraclecloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: oraclecloud.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"symantec.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-platforms/refs/heads/main/security/oracle-platforms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Cloud Computing
- Database
- Enterprise Software
- Infrastructure as a Service
- Integration
- Machine Learning
- Platform as a Service
- SaaS
---
