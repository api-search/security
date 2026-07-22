---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sentisis.com
  spf: true
hosts:
- cert_expires: Oct 15 11:18:22 2026 GMT
  host: sentisis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sentisis Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sentisis Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sentisis Analytics
provider_slug: sentisis-analytics
slug: sentisis-analytics-domain-security
source_filename: sentisis-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sentisis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 11:18:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sentisis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentisis-analytics/refs/heads/main/security/sentisis-analytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Analytics
- Sentiment Analysis
- Social Media Analytics
- Natural Language Processing
- Consumer Intelligence
- Customer Experience
---
