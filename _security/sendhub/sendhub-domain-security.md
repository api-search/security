---
api_specs:
- filename: sendhub-authentication-api-openapi.yml
  format: yaml
  label: SendHub Authentication API
  slug: sendhub-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/openapi/sendhub-authentication-api-openapi.yml
- filename: sendhub-contact-api-openapi.yml
  format: yaml
  label: SendHub Contact API
  slug: sendhub-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/openapi/sendhub-contact-api-openapi.yml
- filename: sendhub-group-api-openapi.yml
  format: yaml
  label: SendHub Group API
  slug: sendhub-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/openapi/sendhub-group-api-openapi.yml
- filename: sendhub-message-api-openapi.yml
  format: yaml
  label: SendHub Message API
  slug: sendhub-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/openapi/sendhub-message-api-openapi.yml
- filename: sendhub-profile-api-openapi.yml
  format: yaml
  label: SendHub Profile API
  slug: sendhub-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/openapi/sendhub-profile-api-openapi.yml
- filename: sendhub-thread-api-openapi.yml
  format: yaml
  label: SendHub Thread API
  slug: sendhub-thread-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/openapi/sendhub-thread-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sendhub.com
  spf: true
hosts:
- cert_expires: Sep  2 20:02:11 2026 GMT
  host: sendhub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: api.sendhub.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sendhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SendHub, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SendHub
provider_slug: sendhub
slug: sendhub-domain-security
source_filename: sendhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sendhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:02:11 2026 GMT\n  hsts: false\n- host: api.sendhub.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: sendhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/security/sendhub-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SMS
- Messaging
- Text Messaging
- Communications
- Marketing
- Webhooks
- VoIP
---
