---
api_specs:
- filename: apache-samza-checkpoints-api-openapi.yml
  format: yaml
  label: Apache Samza Checkpoints API
  slug: apache-samza-checkpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/openapi/apache-samza-checkpoints-api-openapi.yml
- filename: apache-samza-jobs-api-openapi.yml
  format: yaml
  label: Apache Samza Jobs API
  slug: apache-samza-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/openapi/apache-samza-jobs-api-openapi.yml
- filename: apache-samza-tasks-api-openapi.yml
  format: yaml
  label: Apache Samza Tasks API
  slug: apache-samza-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/openapi/apache-samza-tasks-api-openapi.yml
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
  host: samza.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Samza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Samza, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Samza
provider_slug: apache-samza
slug: apache-samza-domain-security
source_filename: apache-samza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: samza.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/security/apache-samza-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Big Data
- Hadoop
- Kafka
- Stream Processing
- Streaming
- Apache
- Open Source
---
