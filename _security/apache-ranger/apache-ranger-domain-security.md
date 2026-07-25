---
api_specs:
- filename: apache-ranger-audit-api-openapi.yml
  format: yaml
  label: Apache Ranger Audit API
  slug: apache-ranger-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/openapi/apache-ranger-audit-api-openapi.yml
- filename: apache-ranger-groups-api-openapi.yml
  format: yaml
  label: Apache Ranger Groups API
  slug: apache-ranger-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/openapi/apache-ranger-groups-api-openapi.yml
- filename: apache-ranger-policies-api-openapi.yml
  format: yaml
  label: Apache Ranger Policies API
  slug: apache-ranger-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/openapi/apache-ranger-policies-api-openapi.yml
- filename: apache-ranger-services-api-openapi.yml
  format: yaml
  label: Apache Ranger Services API
  slug: apache-ranger-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/openapi/apache-ranger-services-api-openapi.yml
- filename: apache-ranger-users-api-openapi.yml
  format: yaml
  label: Apache Ranger Users API
  slug: apache-ranger-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/openapi/apache-ranger-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: ranger.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Ranger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Ranger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Ranger
provider_slug: apache-ranger
slug: apache-ranger-domain-security
source_filename: apache-ranger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ranger.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/security/apache-ranger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
---
