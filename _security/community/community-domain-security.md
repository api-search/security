---
api_specs:
- filename: community-member-data-api-openapi.yml
  format: yaml
  label: Community member-data API
  slug: community-member-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/openapi/community-member-data-api-openapi.yml
- filename: community-messaging-api-openapi.yml
  format: yaml
  label: Community messaging API
  slug: community-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/openapi/community-messaging-api-openapi.yml
- filename: community-tags-api-openapi.yml
  format: yaml
  label: Community tags API
  slug: community-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/openapi/community-tags-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@community.com"
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
- cert_expires: Sep 14 12:04:45 2026 GMT
  host: developer.community.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 15:15:35 2026 GMT
  host: dl.community.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Community Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Community, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Community
provider_slug: community
slug: community-domain-security
source_filename: community-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: community.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:17:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.community.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:04:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dl.community.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 15:15:35 2026 GMT\n  hsts: null\ndomains:\n- domain: community.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@community.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/security/community-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- SMS
- Communications
- Conversational
- Marketing
- Creators
- Webhook
- Company
---
