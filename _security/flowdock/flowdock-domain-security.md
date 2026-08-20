---
api_specs:
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
- filename: flowdock-authentication-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Authentication API
  slug: flowdock-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-authentication-api-openapi.yml
- filename: flowdock-chat-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Chat API
  slug: flowdock-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-chat-api-openapi.yml
- filename: flowdock-files-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Files API
  slug: flowdock-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-files-api-openapi.yml
- filename: flowdock-flows-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Flows API
  slug: flowdock-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-flows-api-openapi.yml
- filename: flowdock-invitations-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Invitations API
  slug: flowdock-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-invitations-api-openapi.yml
- filename: flowdock-messages-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Messages API
  slug: flowdock-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-messages-api-openapi.yml
- filename: flowdock-organizations-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Organizations API
  slug: flowdock-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-organizations-api-openapi.yml
- filename: flowdock-private-conversations-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Private Conversations API
  slug: flowdock-private-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-private-conversations-api-openapi.yml
- filename: flowdock-private-messages-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Private Messages API
  slug: flowdock-private-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-private-messages-api-openapi.yml
- filename: flowdock-sources-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Sources API
  slug: flowdock-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-sources-api-openapi.yml
- filename: flowdock-team-inbox-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Team Inbox API
  slug: flowdock-team-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-team-inbox-api-openapi.yml
- filename: flowdock-threads-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Threads API
  slug: flowdock-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-threads-api-openapi.yml
- filename: flowdock-users-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Users API
  slug: flowdock-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-users-api-openapi.yml
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
- Integration
- Discontinued
---
