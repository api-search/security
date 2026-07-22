---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mentimeter.com
  spf: true
hosts:
- cert_expires: Oct 15 17:45:01 2026 GMT
  host: mentimeter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mentimeter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mentimeter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mentimeter
provider_slug: mentimeter
slug: mentimeter-domain-security
source_filename: mentimeter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mentimeter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 17:45:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mentimeter.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mentimeter/refs/heads/main/security/mentimeter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Presentations
- Audience Engagement
- Live Polling
- Quizzes
- Surveys
- Interactive Presentations
- Education
---
