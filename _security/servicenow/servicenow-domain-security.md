---
api_specs:
- filename: servicenow-events-asyncapi.yml
  format: yaml
  label: ServiceNow Event Management Topic Open API
  slug: servicenow-event-management-topic-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/asyncapi/servicenow-events-asyncapi.yml
- filename: servicenow-aggregate-statistics-api-openapi.yml
  format: yaml
  label: ServiceNow Aggregate Statistics API
  slug: servicenow-aggregate-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-aggregate-statistics-api-openapi.yml
- filename: servicenow-attachments-api-openapi.yml
  format: yaml
  label: ServiceNow Attachments API
  slug: servicenow-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-attachments-api-openapi.yml
- filename: servicenow-cart-api-openapi.yml
  format: yaml
  label: ServiceNow Cart API
  slug: servicenow-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-cart-api-openapi.yml
- filename: servicenow-catalog-items-api-openapi.yml
  format: yaml
  label: ServiceNow Catalog Items API
  slug: servicenow-catalog-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-catalog-items-api-openapi.yml
- filename: servicenow-catalogs-api-openapi.yml
  format: yaml
  label: ServiceNow Catalogs API
  slug: servicenow-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-catalogs-api-openapi.yml
- filename: servicenow-categories-api-openapi.yml
  format: yaml
  label: ServiceNow Categories API
  slug: servicenow-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-categories-api-openapi.yml
- filename: servicenow-change-tasks-api-openapi.yml
  format: yaml
  label: ServiceNow Change Tasks API
  slug: servicenow-change-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-change-tasks-api-openapi.yml
- filename: servicenow-cmdb-instances-api-openapi.yml
  format: yaml
  label: ServiceNow CMDB Instances API
  slug: servicenow-cmdb-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-cmdb-instances-api-openapi.yml
- filename: servicenow-contact-api-openapi.yml
  format: yaml
  label: ServiceNow Contact API
  slug: servicenow-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-contact-api-openapi.yml
- filename: servicenow-emergency-changes-api-openapi.yml
  format: yaml
  label: ServiceNow Emergency Changes API
  slug: servicenow-emergency-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-emergency-changes-api-openapi.yml
- filename: servicenow-import-sets-api-openapi.yml
  format: yaml
  label: ServiceNow Import Sets API
  slug: servicenow-import-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-import-sets-api-openapi.yml
- filename: servicenow-normal-changes-api-openapi.yml
  format: yaml
  label: ServiceNow Normal Changes API
  slug: servicenow-normal-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-normal-changes-api-openapi.yml
- filename: servicenow-standard-changes-api-openapi.yml
  format: yaml
  label: ServiceNow Standard Changes API
  slug: servicenow-standard-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-standard-changes-api-openapi.yml
- filename: servicenow-table-records-api-openapi.yml
  format: yaml
  label: ServiceNow Table Records API
  slug: servicenow-table-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-table-records-api-openapi.yml
- filename: servicenow-trouble-ticket-api-openapi.yml
  format: yaml
  label: ServiceNow Trouble Ticket API
  slug: servicenow-trouble-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-trouble-ticket-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: servicenow.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.servicenow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 07:18:06 2026 GMT
  host: developer.servicenow.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: docs.servicenow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Servicenow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ServiceNow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ServiceNow
provider_slug: servicenow
slug: servicenow-domain-security
source_filename: servicenow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.servicenow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\n- host: developer.servicenow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 07:18:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.servicenow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: servicenow.com\n  dnssec: true\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/security/servicenow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
---
