---
api_specs:
- filename: rss-app-openapi-generated.yml
  format: yaml
  label: RSS.app API
  slug: rss-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rss-app/refs/heads/main/openapi/_ae-authored/rss-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rss.app
  spf: true
hosts:
- cert_expires: Dec  4 01:03:29 2026 GMT
  host: rss.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rss App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RSS.app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: RSS.app
provider_slug: rss-app
slug: rss-app-domain-security
source_filename: rss-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rss.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 01:03:29 2026 GMT\n  hsts: false\ndomains:\n- domain: rss.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rss-app/refs/heads/main/security/rss-app-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- RSS
- No-code
- Automation
- Content
---
