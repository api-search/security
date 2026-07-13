---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: diffbot.com
  spf: true
hosts:
- cert_expires: Aug 27 21:55:32 2026 GMT
  host: www.diffbot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 08:23:12 2026 GMT
  host: docs.diffbot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 21:42:49 2026 GMT
  host: api.diffbot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diffbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diffbot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Diffbot
provider_slug: diffbot
slug: diffbot-domain-security
source_filename: diffbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.diffbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 21:55:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.diffbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 08:23:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.diffbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:42:49 2026 GMT\n  hsts: null\ndomains:\n- domain: diffbot.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diffbot/refs/heads/main/security/diffbot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Extraction
- Harvesting
- Scraping
- Web
---
