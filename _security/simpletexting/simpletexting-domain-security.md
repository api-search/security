---
api_specs:
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Messages API
  slug: messages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Contacts API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Lists API
  slug: lists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Campaigns API
  slug: campaigns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Autoresponders API
  slug: autoresponders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Sending Numbers API
  slug: sending-numbers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
- filename: simpletexting-openapi.yml
  format: yaml
  label: SimpleTexting Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: simpletexting.com
  spf: true
hosts:
- cert_expires: Aug 20 04:06:57 2026 GMT
  host: simpletexting.com
  hsts: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api-doc.simpletexting.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api-app2.simpletexting.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simpletexting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimpleTexting, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SimpleTexting
provider_slug: simpletexting
slug: simpletexting-domain-security
source_filename: simpletexting-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simpletexting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 04:06:57 2026 GMT\n  hsts: true\n- host: api-doc.simpletexting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-app2.simpletexting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: simpletexting.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/security/simpletexting-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SMS
- MMS
- Messaging
- Marketing
- Text Messaging
---
