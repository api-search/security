---
api_specs:
- filename: community-async-openapi-original.yml
  format: yaml
  label: Community Async REST API
  slug: community-async-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/openapi/community-async-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@community.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: community.com
  spf: true
hosts:
- cert_expires: Sep 26 16:17:35 2026 GMT
  host: community.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Community Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Community, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Community
provider_slug: community
slug: community-domain-security
source_filename: community-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: community.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:17:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: community.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@community.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/security/community-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- SMS
- Communications
- Conversational
- Marketing
- Creators
- Webhooks
- Company
---
