---
api_specs:
- filename: apache-openwhisk-actions-api-openapi.yml
  format: yaml
  label: Apache OpenWhisk Actions API
  slug: apache-openwhisk-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/openapi/apache-openwhisk-actions-api-openapi.yml
- filename: apache-openwhisk-activations-api-openapi.yml
  format: yaml
  label: Apache OpenWhisk Activations API
  slug: apache-openwhisk-activations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/openapi/apache-openwhisk-activations-api-openapi.yml
- filename: apache-openwhisk-namespaces-api-openapi.yml
  format: yaml
  label: Apache OpenWhisk Namespaces API
  slug: apache-openwhisk-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/openapi/apache-openwhisk-namespaces-api-openapi.yml
- filename: apache-openwhisk-packages-api-openapi.yml
  format: yaml
  label: Apache OpenWhisk Packages API
  slug: apache-openwhisk-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/openapi/apache-openwhisk-packages-api-openapi.yml
- filename: apache-openwhisk-rules-api-openapi.yml
  format: yaml
  label: Apache OpenWhisk Rules API
  slug: apache-openwhisk-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/openapi/apache-openwhisk-rules-api-openapi.yml
- filename: apache-openwhisk-triggers-api-openapi.yml
  format: yaml
  label: Apache OpenWhisk Triggers API
  slug: apache-openwhisk-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/openapi/apache-openwhisk-triggers-api-openapi.yml
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
  host: openwhisk.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Openwhisk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache OpenWhisk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
slug: apache-openwhisk-domain-security
source_filename: apache-openwhisk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openwhisk.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/security/apache-openwhisk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud-Native
- Event-Driven
- Function-as-a-Service
- Serverless
- Apache
- Open-Source
- Functions
---
