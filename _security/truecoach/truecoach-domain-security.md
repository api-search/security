---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: truecoach.co
  spf: true
hosts:
- cert_expires: Sep 15 07:36:08 2026 GMT
  host: truecoach.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truecoach Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrueCoach, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TrueCoach
provider_slug: truecoach
slug: truecoach-domain-security
source_filename: truecoach-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truecoach.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:36:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: truecoach.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truecoach/refs/heads/main/security/truecoach-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fitness
- Personal Training
- Coaching
- Workouts
- Nutrition
- Health
- SaaS
---
