---
api_specs:
- filename: flowdock-rest-api-openapi.yml
  format: yaml
  label: Flowdock REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-rest-api-openapi.yml
- filename: flowdock-push-api-openapi.yml
  format: yaml
  label: Flowdock Push API (Deprecated)
  slug: push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-push-api-openapi.yml
- filename: flowdock-streaming-api-asyncapi.yml
  format: yaml
  label: Flowdock Streaming API
  slug: streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/asyncapi/flowdock-streaming-api-asyncapi.yml
- filename: flowdock-scim-api-openapi.yml
  format: yaml
  label: Flowdock SCIM Provisioning API
  slug: scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-scim-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: archive.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flowdock.com
  spf: false
hosts:
- cert_expires: Feb  9 22:02:42 2027 GMT
  host: web.archive.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.flowdock.com
  https: false
- host: stream.flowdock.com
  https: false
kind: domain-security
layout: security
method: probed
name: Flowdock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flowdock (Discontinued), probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flowdock (Discontinued)
provider_slug: flowdock
slug: flowdock-domain-security
source_filename: flowdock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: web.archive.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 22:02:42 2027 GMT\n  hsts: false\n- host: api.flowdock.com\n  https: false\n- host: stream.flowdock.com\n  https: false\ndomains:\n- domain: archive.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: flowdock.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/security/flowdock-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Team Chat
- Team Inbox
- Collaboration
- Real-Time Messaging
- Integrations
- Discontinued
---
