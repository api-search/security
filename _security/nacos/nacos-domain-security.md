---
api_specs:
- filename: nacos-auth-api-openapi.yml
  format: yaml
  label: Nacos Auth API
  slug: nacos-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-auth-api-openapi.yml
- filename: nacos-configuration-api-openapi.yml
  format: yaml
  label: Nacos Configuration API
  slug: nacos-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-configuration-api-openapi.yml
- filename: nacos-namespace-api-openapi.yml
  format: yaml
  label: Nacos Namespace API
  slug: nacos-namespace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-namespace-api-openapi.yml
- filename: nacos-operator-api-openapi.yml
  format: yaml
  label: Nacos Operator API
  slug: nacos-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-operator-api-openapi.yml
- filename: nacos-service-discovery-api-openapi.yml
  format: yaml
  label: Nacos Service Discovery API
  slug: nacos-service-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-service-discovery-api-openapi.yml
- filename: nacos-service-management-api-openapi.yml
  format: yaml
  label: Nacos Service Management API
  slug: nacos-service-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-service-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nacos.io
  spf: false
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: nacos.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nacos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nacos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Nacos
provider_slug: nacos
slug: nacos-domain-security
source_filename: nacos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nacos.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nacos.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/security/nacos-domain-security.yml
summary_line: TLSv1.3
tags:
- Alibaba
- Cloud Native
- Configuration Management
- DNS
- Java
- Microservices
- Service Discovery
- Service Management
---
