---
api_specs:
- filename: apache-dubbo-conditionrule-api-openapi.yml
  format: yaml
  label: Apache Dubbo ConditionRule API
  slug: apache-dubbo-conditionrule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-conditionrule-api-openapi.yml
- filename: apache-dubbo-metrics-api-openapi.yml
  format: yaml
  label: Apache Dubbo metrics API
  slug: apache-dubbo-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-metrics-api-openapi.yml
- filename: apache-dubbo-mockrules-api-openapi.yml
  format: yaml
  label: Apache Dubbo MockRules API
  slug: apache-dubbo-mockrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-mockrules-api-openapi.yml
- filename: apache-dubbo-overriderule-api-openapi.yml
  format: yaml
  label: Apache Dubbo OverrideRule API
  slug: apache-dubbo-overriderule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-overriderule-api-openapi.yml
- filename: apache-dubbo-services-api-openapi.yml
  format: yaml
  label: Apache Dubbo Services API
  slug: apache-dubbo-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-services-api-openapi.yml
- filename: apache-dubbo-tagrule-api-openapi.yml
  format: yaml
  label: Apache Dubbo TagRule API
  slug: apache-dubbo-tagrule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-tagrule-api-openapi.yml
- filename: apache-dubbo-trafficaccesslog-api-openapi.yml
  format: yaml
  label: Apache Dubbo TrafficAccesslog API
  slug: apache-dubbo-trafficaccesslog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-trafficaccesslog-api-openapi.yml
- filename: apache-dubbo-trafficargument-api-openapi.yml
  format: yaml
  label: Apache Dubbo TrafficArgument API
  slug: apache-dubbo-trafficargument-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-trafficargument-api-openapi.yml
- filename: apache-dubbo-trafficgray-api-openapi.yml
  format: yaml
  label: Apache Dubbo TrafficGray API
  slug: apache-dubbo-trafficgray-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-trafficgray-api-openapi.yml
- filename: apache-dubbo-trafficmock-api-openapi.yml
  format: yaml
  label: Apache Dubbo TrafficMock API
  slug: apache-dubbo-trafficmock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-trafficmock-api-openapi.yml
- filename: apache-dubbo-trafficregion-api-openapi.yml
  format: yaml
  label: Apache Dubbo TrafficRegion API
  slug: apache-dubbo-trafficregion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-trafficregion-api-openapi.yml
- filename: apache-dubbo-trafficretry-api-openapi.yml
  format: yaml
  label: Apache Dubbo TrafficRetry API
  slug: apache-dubbo-trafficretry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-trafficretry-api-openapi.yml
- filename: apache-dubbo-traffictimeout-api-openapi.yml
  format: yaml
  label: Apache Dubbo TrafficTimeout API
  slug: apache-dubbo-traffictimeout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-traffictimeout-api-openapi.yml
- filename: apache-dubbo-trafficweight-api-openapi.yml
  format: yaml
  label: Apache Dubbo TrafficWeight API
  slug: apache-dubbo-trafficweight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/openapi/apache-dubbo-trafficweight-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:root@apache.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: dubbo.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Apache Dubbo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Dubbo, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Dubbo
provider_slug: apache-dubbo
slug: apache-dubbo-domain-security
source_filename: apache-dubbo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dubbo.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/security/apache-dubbo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache
- Go
- Java
- Microservices
- Open-Source
- RPC
- Service Discovery
- Service Mesh
---
