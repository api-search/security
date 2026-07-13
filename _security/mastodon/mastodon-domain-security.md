---
api_specs:
- filename: mastodon.yml
  format: yaml
  label: Mastodon API
  slug: mastodon
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastodon/refs/heads/main/openapi/mastodon.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joinmastodon.org
  spf: true
hosts:
- cert_expires: Sep 28 00:47:46 2026 GMT
  host: docs.joinmastodon.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mastodon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mastodon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mastodon
provider_slug: mastodon
slug: mastodon-domain-security
source_filename: mastodon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.joinmastodon.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 00:47:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: joinmastodon.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mastodon/refs/heads/main/security/mastodon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open-Source
- Social Networks
---
