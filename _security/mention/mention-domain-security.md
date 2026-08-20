---
api_specs:
- filename: mention-accounts-api-openapi.yml
  format: yaml
  label: Mention Accounts API
  slug: mention-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-accounts-api-openapi.yml
- filename: mention-alerts-api-openapi.yml
  format: yaml
  label: Mention Alerts API
  slug: mention-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-alerts-api-openapi.yml
- filename: mention-authors-api-openapi.yml
  format: yaml
  label: Mention Authors API
  slug: mention-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-authors-api-openapi.yml
- filename: mention-mentions-api-openapi.yml
  format: yaml
  label: Mention Mentions API
  slug: mention-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-mentions-api-openapi.yml
- filename: mention-shares-api-openapi.yml
  format: yaml
  label: Mention Shares API
  slug: mention-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-shares-api-openapi.yml
- filename: mention-stats-api-openapi.yml
  format: yaml
  label: Mention Stats API
  slug: mention-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-stats-api-openapi.yml
- filename: mention-tags-api-openapi.yml
  format: yaml
  label: Mention Tags API
  slug: mention-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-tags-api-openapi.yml
- filename: mention-tasks-api-openapi.yml
  format: yaml
  label: Mention Tasks API
  slug: mention-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-tasks-api-openapi.yml
- filename: mention-app-api-openapi.yml
  format: yaml
  label: Mention App API
  slug: mention-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-app-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mention.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: mention.net
  spf: true
hosts:
- cert_expires: Sep 25 18:13:52 2026 GMT
  host: mention.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:40:23 2026 GMT
  host: dev.mention.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:37:36 2026 GMT
  host: api.mention.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mention Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mention, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mention
provider_slug: mention
slug: mention-domain-security
source_filename: mention-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mention.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 18:13:52 2026 GMT\n  hsts: false\n- host: dev.mention.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:40:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mention.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:37:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mention.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: mention.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/security/mention-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Alerts
- Brand Monitoring
- Media Monitoring
- Social Listening
- Social-Media
- Sentiment Analysis
- Reputation Management
- Influencer Marketing
- Competitive Intelligence
- Streaming
- Marketing
---
