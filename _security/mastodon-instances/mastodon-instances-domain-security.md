---
api_specs:
- filename: mastodon-instances-openapi.yml
  format: yaml
  label: Mastodon Instances API
  slug: mastodon-instances
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastodon-instances/refs/heads/main/openapi/mastodon-instances-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: instances.social
  spf: true
hosts:
- cert_expires: Aug 13 23:41:02 2026 GMT
  host: instances.social
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mastodon Instances Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mastodon Instances, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Mastodon Instances
provider_slug: mastodon-instances
slug: mastodon-instances-domain-security
source_filename: mastodon-instances-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instances.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:41:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: instances.social\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mastodon-instances/refs/heads/main/security/mastodon-instances-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Fediverse
- Mastodon
- Search
- Social
---
