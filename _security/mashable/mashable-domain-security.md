---
api_specs:
- filename: mashable-openapi.yml
  format: yaml
  label: Mashable via News API
  slug: mashable-via-newsapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mashable/refs/heads/main/openapi/mashable-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mashable.com
  spf: true
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: newsapi.org
  spf: true
hosts:
- cert_expires: Oct  7 11:47:50 2026 GMT
  host: mashable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 23:59:59 2026 GMT
  host: newsapi.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mashable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mashable, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mashable
provider_slug: mashable
slug: mashable-domain-security
source_filename: mashable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mashable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 11:47:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: newsapi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mashable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: newsapi.org\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mashable/refs/heads/main/security/mashable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Articles
- Digital Culture
- Headlines
- Media
- News
- Technology News
---
