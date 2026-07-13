---
api_specs:
- filename: facebook-graph-api.yaml
  format: yaml
  label: Facebook Graph API
  slug: facebook-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-graph-api.yaml
- filename: facebook-marketing-api.yaml
  format: yaml
  label: Facebook Marketing API
  slug: facebook-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-marketing-api.yaml
- filename: facebook-instagram-api.yaml
  format: yaml
  label: Instagram API
  slug: instagram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-instagram-api.yaml
- filename: facebook-messenger-api.yaml
  format: yaml
  label: Messenger Platform API
  slug: messenger-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-messenger-api.yaml
- filename: facebook-threads-api.yaml
  format: yaml
  label: Threads API
  slug: threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-threads-api.yaml
- filename: facebook-whatsapp-api.yaml
  format: yaml
  label: WhatsApp Business API
  slug: whatsapp-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-whatsapp-api.yaml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af"
  dmarc: false
  dnssec: false
  domain: threads.net
  spf: true
hosts:
- cert_expires: Jul 19 23:59:59 2026 GMT
  host: graph.threads.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Facebook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Facebook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Facebook
provider_slug: facebook
slug: facebook-domain-security
source_filename: facebook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graph.threads.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: threads.net\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/security/facebook-domain-security.yml
summary_line: TLSv1.3
tags:
- Fortune 500
- Advertising
- Content Publishing
- Messaging
- Social Media
- Social Networking
---
