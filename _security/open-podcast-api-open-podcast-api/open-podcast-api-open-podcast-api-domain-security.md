---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openpodcastapi.org
  spf: true
hosts:
- cert_expires: Sep 24 13:57:00 2026 GMT
  host: openpodcastapi.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Podcast Api Open Podcast Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Podcast API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Open Podcast API
provider_slug: open-podcast-api-open-podcast-api
slug: open-podcast-api-open-podcast-api-domain-security
source_filename: open-podcast-api-open-podcast-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openpodcastapi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 13:57:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openpodcastapi.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-podcast-api-open-podcast-api/refs/heads/main/security/open-podcast-api-open-podcast-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Audio
- Episodes
- Open Standards
- Podcasts
- Subscriptions
- Sync
---
