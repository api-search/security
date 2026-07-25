---
api_specs:
- filename: diaspora-aspects-api-openapi.yml
  format: yaml
  label: Diaspora Aspects API
  slug: diaspora-aspects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-aspects-api-openapi.yml
- filename: diaspora-comments-api-openapi.yml
  format: yaml
  label: Diaspora Comments API
  slug: diaspora-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-comments-api-openapi.yml
- filename: diaspora-contacts-api-openapi.yml
  format: yaml
  label: Diaspora Contacts API
  slug: diaspora-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-contacts-api-openapi.yml
- filename: diaspora-conversations-api-openapi.yml
  format: yaml
  label: Diaspora Conversations API
  slug: diaspora-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-conversations-api-openapi.yml
- filename: diaspora-likes-api-openapi.yml
  format: yaml
  label: Diaspora Likes API
  slug: diaspora-likes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-likes-api-openapi.yml
- filename: diaspora-notifications-api-openapi.yml
  format: yaml
  label: Diaspora Notifications API
  slug: diaspora-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-notifications-api-openapi.yml
- filename: diaspora-photos-api-openapi.yml
  format: yaml
  label: Diaspora Photos API
  slug: diaspora-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-photos-api-openapi.yml
- filename: diaspora-post-interactions-api-openapi.yml
  format: yaml
  label: Diaspora Post interactions API
  slug: diaspora-post-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-post-interactions-api-openapi.yml
- filename: diaspora-posts-api-openapi.yml
  format: yaml
  label: Diaspora Posts API
  slug: diaspora-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-posts-api-openapi.yml
- filename: diaspora-reshares-api-openapi.yml
  format: yaml
  label: Diaspora Reshares API
  slug: diaspora-reshares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-reshares-api-openapi.yml
- filename: diaspora-search-api-openapi.yml
  format: yaml
  label: Diaspora Search API
  slug: diaspora-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-search-api-openapi.yml
- filename: diaspora-streams-api-openapi.yml
  format: yaml
  label: Diaspora Streams API
  slug: diaspora-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-streams-api-openapi.yml
- filename: diaspora-tag-followings-api-openapi.yml
  format: yaml
  label: Diaspora Tag followings API
  slug: diaspora-tag-followings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-tag-followings-api-openapi.yml
- filename: diaspora-users-api-openapi.yml
  format: yaml
  label: Diaspora Users API
  slug: diaspora-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: diasporafoundation.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: diaspora.social
  spf: true
hosts:
- cert_expires: Sep 15 18:21:43 2026 GMT
  host: diasporafoundation.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 05:26:24 2026 GMT
  host: diaspora.social
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diaspora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diaspora, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Diaspora
provider_slug: diaspora
slug: diaspora-domain-security
source_filename: diaspora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: diasporafoundation.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 18:21:43 2026 GMT\n  hsts: false\n- host: diaspora.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 05:26:24 2026 GMT\n  hsts: false\ndomains:\n- domain: diasporafoundation.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: diaspora.social\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/security/diaspora-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Social
- Social Networking
- Decentralized
- Federated
- Open Source
- Privacy
- Fediverse
- Messaging
- OpenID Connect
---
