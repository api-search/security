---
api_specs:
- filename: eventmesh-messaging.yml
  format: yaml
  label: Apache EventMesh Messaging API
  slug: eventmesh-messaging-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/asyncapi/eventmesh-messaging.yml
- filename: apache-event-mesh-client-api-openapi.yml
  format: yaml
  label: Apache EventMesh Client API
  slug: apache-event-mesh-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/openapi/apache-event-mesh-client-api-openapi.yml
- filename: apache-event-mesh-event-api-openapi.yml
  format: yaml
  label: Apache EventMesh Event API
  slug: apache-event-mesh-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/openapi/apache-event-mesh-event-api-openapi.yml
- filename: apache-event-mesh-monitoring-api-openapi.yml
  format: yaml
  label: Apache EventMesh Monitoring API
  slug: apache-event-mesh-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/openapi/apache-event-mesh-monitoring-api-openapi.yml
- filename: apache-event-mesh-registry-api-openapi.yml
  format: yaml
  label: Apache EventMesh Registry API
  slug: apache-event-mesh-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/openapi/apache-event-mesh-registry-api-openapi.yml
- filename: apache-event-mesh-subscription-api-openapi.yml
  format: yaml
  label: Apache EventMesh Subscription API
  slug: apache-event-mesh-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/openapi/apache-event-mesh-subscription-api-openapi.yml
- filename: apache-event-mesh-topic-api-openapi.yml
  format: yaml
  label: Apache EventMesh Topic API
  slug: apache-event-mesh-topic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/openapi/apache-event-mesh-topic-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: eventmesh.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Event Mesh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache EventMesh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache EventMesh
provider_slug: apache-event-mesh
slug: apache-event-mesh-domain-security
source_filename: apache-event-mesh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eventmesh.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/security/apache-event-mesh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache
- CloudEvents
- Event-Driven
- Messaging
- Open Source
- Pub-Sub
- Serverless
---
