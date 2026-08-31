---
api_specs:
- filename: apache-nifi-access-api-openapi.yml
  format: yaml
  label: Apache NiFi Access API
  slug: apache-nifi-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nifi/refs/heads/main/openapi/apache-nifi-access-api-openapi.yml
- filename: apache-nifi-connections-api-openapi.yml
  format: yaml
  label: Apache NiFi Connections API
  slug: apache-nifi-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nifi/refs/heads/main/openapi/apache-nifi-connections-api-openapi.yml
- filename: apache-nifi-controller-services-api-openapi.yml
  format: yaml
  label: Apache NiFi Controller Services API
  slug: apache-nifi-controller-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nifi/refs/heads/main/openapi/apache-nifi-controller-services-api-openapi.yml
- filename: apache-nifi-flow-api-openapi.yml
  format: yaml
  label: Apache NiFi Flow API
  slug: apache-nifi-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nifi/refs/heads/main/openapi/apache-nifi-flow-api-openapi.yml
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
  host: nifi.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Nifi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache NiFi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache NiFi
provider_slug: apache-nifi
slug: apache-nifi-domain-security
source_filename: apache-nifi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nifi.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-nifi/refs/heads/main/security/apache-nifi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Integration
- Dataflow
- ETL
- IoT
- Streaming
- Data Pipeline
---
