---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: life-is-tech.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lifeistech-lesson.jp
  spf: false
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: life-is-tech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: camp.life-is-tech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: members.life-is-tech.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 09:43:10 2026 GMT
  host: dx.life-is-tech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: lifeistech-lesson.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Life Is Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Life is Tech, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Life is Tech
provider_slug: life-is-tech
slug: life-is-tech-domain-security
source_filename: life-is-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts and the company's public product hosts\nnote: >-\n  Life is Tech publishes no API host, so there are no OpenAPI servers[] to probe. The hosts\n  below are the corporate site and the four public product sites linked from the homepage.\nhosts:\n- host: life-is-tech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n- host: camp.life-is-tech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n- host: members.life-is-tech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dx.life-is-tech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 09:43:10 2026 GMT\n  hsts: false\n- host: lifeistech-lesson.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\n\
  domains:\n- domain: life-is-tech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: lifeistech-lesson.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/life-is-tech/refs/heads/main/security/life-is-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Learning
- Training
- Programming Education
- Digital Skills
- Japan
---
