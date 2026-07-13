---
api_specs:
- filename: knowledgeapi.yaml
  format: yaml
  label: Yext Knowledge API
  slug: yext-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/knowledgeapi.yaml
- filename: answersapi.yaml
  format: yaml
  label: Yext Answers API
  slug: yext-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/answersapi.yaml
- filename: chatapi.yaml
  format: yaml
  label: Yext Chat API
  slug: yext-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/chatapi.yaml
- filename: eventsapi.yaml
  format: yaml
  label: Yext Events API
  slug: yext-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/eventsapi.yaml
- filename: liveapi.yaml
  format: yaml
  label: Yext Live API
  slug: yext-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/liveapi.yaml
- filename: adminapi.yaml
  format: yaml
  label: Yext Admin API
  slug: yext-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/adminapi.yaml
- filename: publisherlistingsapi.yaml
  format: yaml
  label: Yext Publisher Listings API
  slug: yext-publisher-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/publisherlistingsapi.yaml
- filename: publishereclapi.yaml
  format: yaml
  label: Yext Publisher ECL API
  slug: yext-publisher-ecl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/publishereclapi.yaml
- filename: publishernotifyreviewapi.yaml
  format: yaml
  label: Yext Publisher Notify Review API
  slug: yext-publisher-notify-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/publishernotifyreviewapi.yaml
- filename: publishertrackingpixelapi.yaml
  format: yaml
  label: Yext Publisher Tracking Pixel API
  slug: yext-publisher-tracking-pixel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/publishertrackingpixelapi.yaml
- filename: webhooks.yaml
  format: yaml
  label: Yext Webhooks
  slug: yext-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/webhooks.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yext.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: yextapis.com
  spf: false
hosts:
- cert_expires: Oct  7 01:51:55 2026 GMT
  host: www.yext.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 13:41:45 2026 GMT
  host: hitchhikers.yext.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 16:43:41 2026 GMT
  host: api.yextapis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yext, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yext
provider_slug: yext
slug: yext-domain-security
source_filename: yext-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 01:51:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: hitchhikers.yext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:41:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.yextapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:43:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yext.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: yextapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yext/refs/heads/main/security/yext-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Presence
- Business Listings
- Location Data
- Reviews
- AI Search
- Knowledge Graph
---
