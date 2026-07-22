---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: labster.com
  spf: true
hosts:
- cert_expires: Sep 11 15:40:00 2026 GMT
  host: www.labster.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Labster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Labster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Labster
provider_slug: labster
slug: labster-domain-security
source_filename: labster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.labster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:40:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: labster.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/labster/refs/heads/main/security/labster-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Virtual Labs
- Science Education
- STEM
- Simulation
- Learning Management System
- LTI
- Higher Education
---
