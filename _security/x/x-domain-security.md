---
api_specs:
- filename: x-account-activity-api-openapi.yml
  format: yaml
  label: X Account Activity API
  slug: x-account-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-account-activity-api-openapi.yml
- filename: x-account-api-openapi.yml
  format: yaml
  label: X Account API
  slug: x-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-account-api-openapi.yml
- filename: x-activity-api-openapi.yml
  format: yaml
  label: X Activity API
  slug: x-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-activity-api-openapi.yml
- filename: x-articles-api-openapi.yml
  format: yaml
  label: X Articles API
  slug: x-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-articles-api-openapi.yml
- filename: x-bots-api-openapi.yml
  format: yaml
  label: X Bots API
  slug: x-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-bots-api-openapi.yml
- filename: x-broadcasts-api-openapi.yml
  format: yaml
  label: X Broadcasts API
  slug: x-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-broadcasts-api-openapi.yml
- filename: x-chat-api-openapi.yml
  format: yaml
  label: X Chat API
  slug: x-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-chat-api-openapi.yml
- filename: x-communities-api-openapi.yml
  format: yaml
  label: X Communities API
  slug: x-communities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-communities-api-openapi.yml
- filename: x-community-notes-api-openapi.yml
  format: yaml
  label: X Community Notes API
  slug: x-community-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-community-notes-api-openapi.yml
- filename: x-compliance-api-openapi.yml
  format: yaml
  label: X Compliance API
  slug: x-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-compliance-api-openapi.yml
- filename: x-connections-api-openapi.yml
  format: yaml
  label: X Connections API
  slug: x-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-connections-api-openapi.yml
- filename: x-direct-messages-api-openapi.yml
  format: yaml
  label: X Direct Messages API
  slug: x-direct-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-direct-messages-api-openapi.yml
- filename: x-general-api-openapi.yml
  format: yaml
  label: X General API
  slug: x-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-general-api-openapi.yml
- filename: x-lists-api-openapi.yml
  format: yaml
  label: X Lists API
  slug: x-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-lists-api-openapi.yml
- filename: x-media-api-openapi.yml
  format: yaml
  label: X Media API
  slug: x-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-media-api-openapi.yml
- filename: x-news-api-openapi.yml
  format: yaml
  label: X News API
  slug: x-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-news-api-openapi.yml
- filename: x-posts-api-openapi.yml
  format: yaml
  label: X Posts API
  slug: x-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-posts-api-openapi.yml
- filename: x-spaces-api-openapi.yml
  format: yaml
  label: X Spaces API
  slug: x-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-spaces-api-openapi.yml
- filename: x-stream-api-openapi.yml
  format: yaml
  label: X Stream API
  slug: x-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-stream-api-openapi.yml
- filename: x-trends-api-openapi.yml
  format: yaml
  label: X Trends API
  slug: x-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-trends-api-openapi.yml
- filename: x-usage-api-openapi.yml
  format: yaml
  label: X Usage API
  slug: x-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-usage-api-openapi.yml
- filename: x-users-api-openapi.yml
  format: yaml
  label: X Users API
  slug: x-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-users-api-openapi.yml
- filename: x-webhooks-api-openapi.yml
  format: yaml
  label: X Webhooks API
  slug: x-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-webhooks-api-openapi.yml
description: 'Domain-level security posture for the hosts X serves its API and developer surface from. Probed by hand rather than by 0-working/probe-domain-security.py: that tool''s shared provider_hosts() helper carries a global EXCLUDE list containing x.com (there to strip social-profile links from other providers'' apis.yml files), so for THIS provider it discards every real host and returns no-hosts. The finding is about our tooling, not about X. Absence of a record below is a real absence, not an unchecked field.'
domains: []
hosts:
- caa: false
  dnssec: false
  host: x.com
  hsts: true
  hsts_header: max-age=631138519; includeSubdomains
  hsts_preload: false
  http_status: 200
  role: web application, security.txt
  server: cloudflare envoy
  tls: true
- caa: false
  caa_note: api.x.com is a CNAME to dynamic.x.com.cdn.cloudflare.net; no CAA record is published at the name or resolved through the alias chain.
  dnssec: false
  host: api.x.com
  hsts: true
  hsts_header: max-age=631138519; includeSubdomains
  http_status: 404
  http_status_note: The bare host root 404s by design; /2/openapi.json on the same host returns 200.
  role: API base (OpenAPI servers[], MCP endpoint, OAuth token endpoint)
  server: cloudflare envoy
  tls: true
- caa: false
  dnssec: false
  host: developer.x.com
  hsts: true
  hsts_header: max-age=631138519; includeSubdomains
  http_status: 200
  role: developer portal, status page, developer terms
  server: cloudflare envoy
  tls: true
- caa: true
  caa_issuers:
  - letsencrypt.org
  - pki.goog
  - sectigo.com
  - globalsign.com
  caa_note: The only host in the set with CAA, and it comes from the Vercel platform (cname.vercel-dns.com) rather than from X. Note this is where the agent card and agent skill live — X's agent-facing discovery surface sits on third-party hosting.
  dnssec: false
  host: docs.x.com
  hsts: true
  hsts_header: max-age=63072000
  http_status: 308
  role: documentation, llms.txt, agent card, agent skill, docs MCP
  server: Vercel
  tls: true
kind: domain-security
layout: security
method: probed
name: X Domain Security
name_suffix: Domain Security
overview: Domain security posture for X, probed live across 4 host(s) and 0 registrable domain(s).
provider_name: X
provider_slug: x
slug: x-domain-security
source_filename: x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: direct DNS (dig) and TLS/HTTP header probes, 2026-08-28\ndescription: >-\n  Domain-level security posture for the hosts X serves its API and developer surface from.\n  Probed by hand rather than by 0-working/probe-domain-security.py: that tool's shared\n  provider_hosts() helper carries a global EXCLUDE list containing x.com (there to strip\n  social-profile links from other providers' apis.yml files), so for THIS provider it\n  discards every real host and returns no-hosts. The finding is about our tooling, not\n  about X. Absence of a record below is a real absence, not an unchecked field.\nwebsite: x.com\nhosts:\n- host: x.com\n  role: web application, security.txt\n  tls: true\n  hsts: true\n  hsts_header: max-age=631138519; includeSubdomains\n  hsts_preload: false\n  server: cloudflare envoy\n  caa: false\n  dnssec: false\n  http_status: 200\n- host: api.x.com\n  role: API base (OpenAPI servers[], MCP endpoint, OAuth token\
  \ endpoint)\n  tls: true\n  hsts: true\n  hsts_header: max-age=631138519; includeSubdomains\n  server: cloudflare envoy\n  caa: false\n  caa_note: >-\n    api.x.com is a CNAME to dynamic.x.com.cdn.cloudflare.net; no CAA record is published at\n    the name or resolved through the alias chain.\n  dnssec: false\n  http_status: 404\n  http_status_note: The bare host root 404s by design; /2/openapi.json on the same host returns 200.\n- host: developer.x.com\n  role: developer portal, status page, developer terms\n  tls: true\n  hsts: true\n  hsts_header: max-age=631138519; includeSubdomains\n  server: cloudflare envoy\n  caa: false\n  dnssec: false\n  http_status: 200\n- host: docs.x.com\n  role: documentation, llms.txt, agent card, agent skill, docs MCP\n  tls: true\n  hsts: true\n  hsts_header: max-age=63072000\n  server: Vercel\n  caa: true\n  caa_issuers: [letsencrypt.org, pki.goog, sectigo.com, globalsign.com]\n  caa_note: >-\n    The only host in the set with CAA, and it comes from the\
  \ Vercel platform\n    (cname.vercel-dns.com) rather than from X. Note this is where the agent card and agent\n    skill live — X's agent-facing discovery surface sits on third-party hosting.\n  dnssec: false\n  http_status: 308\nemail:\n  domain: x.com\n  spf: true\n  spf_record: >-\n    v=spf1 ip4:199.16.156.0/22 ip4:199.59.148.0/22 include:_spf.google.com\n    include:_spf.salesforce.com include:_oerp.x.com include:phx1.rp.oracleemaildelivery.com\n    include:iad1.rp.oracleemaildelivery.com -all\n  spf_policy: '-all (hard fail)'\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: 'v=DMARC1; p=reject; rua=mailto:...@dmarc-reports.cloudflare.net'\ndnssec:\n  enabled: false\n  note: No DS record is published for x.com; the zone is unsigned.\nsummary:\n  tls: 4/4 hosts\n  hsts: 4/4 hosts\n  hsts_includesubdomains: 3/4 hosts (docs.x.com omits it)\n  caa: 1/4 hosts (docs.x.com only, platform-supplied)\n  dnssec: 0/4 hosts\n  spf: true\n  dmarc: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/security/x-domain-security.yml
summary_line: HSTS
tags:
- Social
- Social Media
- Posts
- Users
- Direct Messages
- Streaming
- Webhooks
- Real Time
- Trends
- Media
- Spaces
- Content
- Conversation
- Agents
- MCP
---
