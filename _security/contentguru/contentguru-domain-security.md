---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: contentguru.com
  spf: true
hosts:
- cert_expires: Dec 23 01:18:53 2026 GMT
  host: www.contentguru.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contentguru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contentguru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Contentguru
provider_slug: contentguru
slug: contentguru-domain-security
source_filename: contentguru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.contentguru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 01:18:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: contentguru.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contentguru/refs/heads/main/security/contentguru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CX
- Cloud
- AI
- Communications
---
