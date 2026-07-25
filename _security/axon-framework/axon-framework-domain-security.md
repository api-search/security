---
api_specs:
- filename: axon-framework-applications-api-openapi.yml
  format: yaml
  label: Axon Framework Applications API
  slug: axon-framework-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/openapi/axon-framework-applications-api-openapi.yml
- filename: axon-framework-cluster-api-openapi.yml
  format: yaml
  label: Axon Framework Cluster API
  slug: axon-framework-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/openapi/axon-framework-cluster-api-openapi.yml
- filename: axon-framework-commands-api-openapi.yml
  format: yaml
  label: Axon Framework Commands API
  slug: axon-framework-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/openapi/axon-framework-commands-api-openapi.yml
- filename: axon-framework-contexts-api-openapi.yml
  format: yaml
  label: Axon Framework Contexts API
  slug: axon-framework-contexts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/openapi/axon-framework-contexts-api-openapi.yml
- filename: axon-framework-event-processors-api-openapi.yml
  format: yaml
  label: Axon Framework Event Processors API
  slug: axon-framework-event-processors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/openapi/axon-framework-event-processors-api-openapi.yml
- filename: axon-framework-events-api-openapi.yml
  format: yaml
  label: Axon Framework Events API
  slug: axon-framework-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/openapi/axon-framework-events-api-openapi.yml
- filename: axon-framework-queries-api-openapi.yml
  format: yaml
  label: Axon Framework Queries API
  slug: axon-framework-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/openapi/axon-framework-queries-api-openapi.yml
- filename: axon-framework-snapshots-api-openapi.yml
  format: yaml
  label: Axon Framework Snapshots API
  slug: axon-framework-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/openapi/axon-framework-snapshots-api-openapi.yml
- filename: axon-framework-users-api-openapi.yml
  format: yaml
  label: Axon Framework Users API
  slug: axon-framework-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/openapi/axon-framework-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: axoniq.io
  spf: true
hosts:
- cert_expires: Aug 25 18:43:52 2026 GMT
  host: www.axoniq.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axon Framework Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axon Framework, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Axon Framework
provider_slug: axon-framework
slug: axon-framework-domain-security
source_filename: axon-framework-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axoniq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 18:43:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axoniq.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/security/axon-framework-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CQRS
- Event Sourcing
- Event-Driven
- Java
- Messaging
- Microservices
---
