---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coursehero.com
  spf: true
hosts:
- cert_expires: Oct  8 21:53:12 2026 GMT
  host: www.coursehero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Course Hero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Course Hero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Course Hero
provider_slug: course-hero
slug: course-hero-domain-security
source_filename: course-hero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coursehero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 21:53:12 2026 GMT\n  hsts: null\ndomains:\n- domain: coursehero.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/course-hero/refs/heads/main/security/course-hero-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Edtech
- Education
- Learning
- Study Resources
- Tutoring
- AI
- Consumer
---
