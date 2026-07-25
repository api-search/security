---
api_specs:
- filename: apache-zipkin-autocomplete-api-openapi.yml
  format: yaml
  label: Apache Zipkin autocomplete API
  slug: apache-zipkin-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-zipkin/refs/heads/main/openapi/apache-zipkin-autocomplete-api-openapi.yml
- filename: apache-zipkin-services-api-openapi.yml
  format: yaml
  label: Apache Zipkin services API
  slug: apache-zipkin-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-zipkin/refs/heads/main/openapi/apache-zipkin-services-api-openapi.yml
- filename: apache-zipkin-spans-api-openapi.yml
  format: yaml
  label: Apache Zipkin spans API
  slug: apache-zipkin-spans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-zipkin/refs/heads/main/openapi/apache-zipkin-spans-api-openapi.yml
- filename: apache-zipkin-traces-api-openapi.yml
  format: yaml
  label: Apache Zipkin traces API
  slug: apache-zipkin-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-zipkin/refs/heads/main/openapi/apache-zipkin-traces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zipkin.io
  spf: false
hosts:
- cert_expires: Sep 30 08:16:22 2026 GMT
  host: zipkin.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Zipkin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Zipkin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Apache Zipkin
provider_slug: apache-zipkin
slug: apache-zipkin-domain-security
source_filename: apache-zipkin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zipkin.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 08:16:22 2026 GMT\n  hsts: false\ndomains:\n- domain: zipkin.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-zipkin/refs/heads/main/security/apache-zipkin-domain-security.yml
summary_line: TLSv1.3
tags:
- Distributed Tracing
- Microservices
- Monitoring
- Observability
- Open Source
---
