---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Oracle REST Data Services (ORDS)
  slug: oracle-rest-data-services-ords
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/
- filename: openapi.yaml
  format: yaml
  label: Oracle Cloud Infrastructure Database API
  slug: oracle-cloud-infrastructure-database-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/iaas/api/#/en/database/
- filename: oracle-database-soda-openapi.yml
  format: yaml
  label: Oracle SODA (Simple Oracle Document Access)
  slug: oracle-soda-simple-oracle-document-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-database/refs/heads/main/openapi/oracle-database-soda-openapi.yml
- filename: oracle-database-txeventq-asyncapi.yml
  format: yaml
  label: Oracle Transactional Event Queues (TxEventQ)
  slug: oracle-transactional-event-queues-txeventq
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-database/refs/heads/main/asyncapi/oracle-database-txeventq-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.oracle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Database Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Database, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Database
provider_slug: oracle-database
slug: oracle-database-domain-security
source_filename: oracle-database-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-database/refs/heads/main/security/oracle-database-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Database
- Enterprise
- Oracle
- REST API
- SQL
---
