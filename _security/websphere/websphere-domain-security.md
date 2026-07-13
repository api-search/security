---
api_specs:
- filename: 9.0.5
  format: yaml
  label: WebSphere Application Server Admin API
  slug: websphere-admin-rest-api
  spec_type: OpenAPI
  url: https://www.ibm.com/docs/en/was/9.0.5?topic=api-openapi-specification
- filename: websphere-liberty-admin-rest-api.yml
  format: yaml
  label: WebSphere Liberty Admin REST API
  slug: websphere-liberty-admin-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/openapi/websphere-liberty-admin-rest-api.yml
- filename: websphere-liberty-rest-connector-api.yml
  format: yaml
  label: WebSphere Liberty REST Connector API
  slug: websphere-liberty-rest-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/openapi/websphere-liberty-rest-connector-api.yml
- filename: websphere-mq-rest-api.yml
  format: yaml
  label: WebSphere MQ REST API
  slug: websphere-mq-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/openapi/websphere-mq-rest-api.yml
- filename: websphere-liberty-collective-controller-rest-api.yml
  format: yaml
  label: WebSphere Liberty Collective Controller REST API
  slug: websphere-liberty-collective-controller-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/openapi/websphere-liberty-collective-controller-rest-api.yml
- filename: websphere-automation-rest-api.yml
  format: yaml
  label: WebSphere Automation REST API
  slug: websphere-automation-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/openapi/websphere-automation-rest-api.yml
- filename: open-liberty-apis.yml
  format: yaml
  label: Open Liberty APIs
  slug: open-liberty-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/openapi/open-liberty-apis.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ibm.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openliberty.io
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: developer.ibm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.ibm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 15:38:16 2026 GMT
  host: openliberty.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Websphere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IBM WebSphere, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IBM WebSphere
provider_slug: websphere
slug: websphere-domain-security
source_filename: websphere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ibm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ibm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openliberty.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 15:38:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ibm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: openliberty.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/security/websphere-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
---
