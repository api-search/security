---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: webz.io
  spf: true
hosts:
- cert_expires: Nov 13 12:21:03 2026 GMT
  host: docs.webz.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 06:49:24 2026 GMT
  host: api.webz.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Webz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webz.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Webz.io
provider_slug: webz
slug: webz-domain-security
source_filename: webz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.webz.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 12:21:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.webz.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 06:49:24 2026 GMT\n  hsts: false\ndomains:\n- domain: webz.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webz/refs/heads/main/security/webz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- News Data
- Web Data
- Web Scraping
- Dark Web
- deep-web
- Cybersecurity
- Threat Intelligence
- Data Breach
- pii-monitoring
- OSINT
- reviews-data
- AI Training Data
- Media Monitoring
---
