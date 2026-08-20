---
api_specs:
- filename: micronaut-beans-api-openapi.yml
  format: yaml
  label: Micronaut Beans API
  slug: micronaut-beans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micronaut/refs/heads/main/openapi/micronaut-beans-api-openapi.yml
- filename: micronaut-configuration-api-openapi.yml
  format: yaml
  label: Micronaut Configuration API
  slug: micronaut-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micronaut/refs/heads/main/openapi/micronaut-configuration-api-openapi.yml
- filename: micronaut-environment-api-openapi.yml
  format: yaml
  label: Micronaut Environment API
  slug: micronaut-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micronaut/refs/heads/main/openapi/micronaut-environment-api-openapi.yml
- filename: micronaut-health-api-openapi.yml
  format: yaml
  label: Micronaut Health API
  slug: micronaut-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micronaut/refs/heads/main/openapi/micronaut-health-api-openapi.yml
- filename: micronaut-info-api-openapi.yml
  format: yaml
  label: Micronaut Info API
  slug: micronaut-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micronaut/refs/heads/main/openapi/micronaut-info-api-openapi.yml
- filename: micronaut-jvm-api-openapi.yml
  format: yaml
  label: Micronaut JVM API
  slug: micronaut-jvm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micronaut/refs/heads/main/openapi/micronaut-jvm-api-openapi.yml
- filename: micronaut-lifecycle-api-openapi.yml
  format: yaml
  label: Micronaut Lifecycle API
  slug: micronaut-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micronaut/refs/heads/main/openapi/micronaut-lifecycle-api-openapi.yml
- filename: micronaut-loggers-api-openapi.yml
  format: yaml
  label: Micronaut Loggers API
  slug: micronaut-loggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micronaut/refs/heads/main/openapi/micronaut-loggers-api-openapi.yml
- filename: micronaut-metrics-api-openapi.yml
  format: yaml
  label: Micronaut Metrics API
  slug: micronaut-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micronaut/refs/heads/main/openapi/micronaut-metrics-api-openapi.yml
- filename: micronaut-routes-api-openapi.yml
  format: yaml
  label: Micronaut Routes API
  slug: micronaut-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micronaut/refs/heads/main/openapi/micronaut-routes-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:admin@websanity.com"
  - 128 iodef "mailto:admin@websanity.com"
  - 128 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: micronaut.io
  spf: true
hosts:
- cert_expires: Oct  3 20:31:53 2026 GMT
  host: micronaut.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Micronaut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Micronaut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Micronaut
provider_slug: micronaut
slug: micronaut-domain-security
source_filename: micronaut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: micronaut.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:31:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: micronaut.io\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:admin@websanity.com\"\n  - 128 iodef \"mailto:admin@websanity.com\"\n  - 128 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/micronaut/refs/heads/main/security/micronaut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud-Native
- Frameworks
- Java
- JVM
- Microservices
- Serverless
---
