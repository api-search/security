---
api_specs:
- filename: spaceflight-news-api-openapi.yml
  format: yaml
  label: Spaceflight News API
  slug: spaceflight-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceflight-news-api/refs/heads/main/openapi/spaceflight-news-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spaceflightnewsapi.net
  spf: true
hosts:
- cert_expires: Aug 19 21:46:58 2026 GMT
  host: www.spaceflightnewsapi.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 20:28:37 2026 GMT
  host: api.spaceflightnewsapi.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spaceflight News Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spaceflight News API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spaceflight News API
provider_slug: spaceflight-news-api
slug: spaceflight-news-api-domain-security
source_filename: spaceflight-news-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spaceflightnewsapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:46:58 2026 GMT\n  hsts: false\n- host: api.spaceflightnewsapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:28:37 2026 GMT\n  hsts: null\ndomains:\n- domain: spaceflightnewsapi.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spaceflight-news-api/refs/heads/main/security/spaceflight-news-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- News
- Space
- Spaceflight
- Media
---
