---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mpds.io
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: mpds.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Materials Platform For Data Science Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Materials Platform for Data Science, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Materials Platform for Data Science
provider_slug: materials-platform-for-data-science
slug: materials-platform-for-data-science-domain-security
source_filename: materials-platform-for-data-science-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mpds.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: mpds.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/materials-platform-for-data-science/refs/heads/main/security/materials-platform-for-data-science-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Science And Math
- Public APIs
---
