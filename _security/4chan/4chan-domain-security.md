---
api_specs:
- filename: 4chan-api.yml
  format: yaml
  label: 4chan Read-Only JSON API
  slug: 4chan-read-only-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4chan/refs/heads/main/openapi/4chan-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: 4chan.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 4cdn.org
  spf: true
hosts:
- cert_expires: Oct  5 13:22:49 2026 GMT
  host: www.4chan.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 03:56:17 2026 GMT
  host: a.4cdn.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 4Chan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4chan, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: 4chan
provider_slug: 4chan
slug: 4chan-domain-security
source_filename: 4chan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.4chan.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 13:22:49 2026 GMT\n  hsts: null\n- host: a.4cdn.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 03:56:17 2026 GMT\n  hsts: null\ndomains:\n- domain: 4chan.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: 4cdn.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4chan/refs/heads/main/security/4chan-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Social
- Bulletin Board
- Imageboard
- Read Only
- JSON
- Public APIs
- Community
---
