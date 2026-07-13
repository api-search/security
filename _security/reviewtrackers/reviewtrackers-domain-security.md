---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reviewtrackers.com
  spf: true
hosts:
- cert_expires: Sep 17 17:03:47 2026 GMT
  host: www.reviewtrackers.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: app.reviewtrackers.com
  hsts: true
  hsts_max_age: 10886400000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reviewtrackers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReviewTrackers, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ReviewTrackers
provider_slug: reviewtrackers
slug: reviewtrackers-domain-security
source_filename: reviewtrackers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reviewtrackers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 17:03:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.reviewtrackers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400000\ndomains:\n- domain: reviewtrackers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reviewtrackers/refs/heads/main/security/reviewtrackers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Reputation Management
- Review Monitoring
- Customer Feedback
- Sentiment Analytics
- Local SEO
- Online Reviews
---
