---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getrewired.org
  spf: true
hosts:
- cert_expires: Jan 10 13:05:23 2027 GMT
  host: getrewired.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LOCK IN Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LOCK IN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LOCK IN
provider_slug: getrewired-org
slug: getrewired-org-domain-security
source_filename: getrewired-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getrewired.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 13:05:23 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getrewired.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getrewired-org/security/getrewired-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health
- Productivity
- iOS
- Wellness
---
