---
api_specs:
- filename: symphony-pod-api-openapi.yml
  format: yaml
  label: Symphony Pod API
  slug: symphony-pod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-pod-api-openapi.yml
- filename: agent-openapi-original.yml
  format: yaml
  label: Symphony Agent API
  slug: symphony-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/agent-openapi-original.yml
- filename: authenticator-openapi-original.yml
  format: yaml
  label: Symphony Authenticator API
  slug: symphony-authenticator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/authenticator-openapi-original.yml
- filename: login-openapi-original.yml
  format: yaml
  label: Symphony Login API
  slug: symphony-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/login-openapi-original.yml
- filename: profile-manager-openapi-original.yml
  format: yaml
  label: Symphony Profile Manager API
  slug: symphony-profile-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/profile-manager-openapi-original.yml
- filename: community-connect-openapi-original.yml
  format: yaml
  label: Symphony Community Connect API
  slug: symphony-community-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/community-connect-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: symphony.com
  spf: true
hosts:
- cert_expires: Sep 30 03:48:59 2026 GMT
  host: symphony.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 30 03:48:59 2026 GMT
  host: developers.symphony.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.2
- host: acme.symphony.com
  https: false
kind: domain-security
layout: security
method: probed
name: Symphony Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Symphony, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Symphony
provider_slug: symphony
slug: symphony-domain-security
source_filename: symphony-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: symphony.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 03:48:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.symphony.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 03:48:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: acme.symphony.com\n  https: false\ndomains:\n- domain: symphony.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/security/symphony-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Collaboration
- Communication
- Financial Services
- Messaging
- Secure Communication
---
