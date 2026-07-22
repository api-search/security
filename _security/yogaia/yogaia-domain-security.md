---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yogaia.com
  spf: true
hosts:
- cert_expires: Oct  9 00:27:52 2026 GMT
  host: yogaia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yogaia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yogaia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Yogaia
provider_slug: yogaia
slug: yogaia-domain-security
source_filename: yogaia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yogaia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 00:27:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yogaia.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yogaia/refs/heads/main/security/yogaia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Yoga
- Fitness
- Wellness
- Online Classes
- Subscription
- Consumer
- Streaming Video
---
