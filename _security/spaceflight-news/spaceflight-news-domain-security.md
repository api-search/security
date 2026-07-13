---
api_specs:
- filename: spaceflight-news-openapi.yml
  format: yaml
  label: Spaceflight News API v4
  slug: spaceflight-news-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceflight-news/refs/heads/main/openapi/spaceflight-news-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spaceflightnewsapi.net
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: thespacedevs.com
  spf: true
hosts:
- cert_expires: Aug 21 09:23:58 2026 GMT
  host: spaceflightnewsapi.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 20:28:37 2026 GMT
  host: api.spaceflightnewsapi.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 05:16:03 2026 GMT
  host: thespacedevs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spaceflight News Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spaceflight News, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spaceflight News
provider_slug: spaceflight-news
slug: spaceflight-news-domain-security
source_filename: spaceflight-news-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spaceflightnewsapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 09:23:58 2026 GMT\n  hsts: false\n- host: api.spaceflightnewsapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:28:37 2026 GMT\n  hsts: null\n- host: thespacedevs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:16:03 2026 GMT\n  hsts: false\ndomains:\n- domain: spaceflightnewsapi.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: thespacedevs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spaceflight-news/refs/heads/main/security/spaceflight-news-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- News
- Space
- Spaceflight
- Aerospace
- Open Source
- Launches
- Public APIs
---
