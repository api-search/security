---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: stepsize.com
  spf: true
hosts:
- cert_expires: Jan 24 18:16:12 2027 GMT
  host: stepsize.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stepsize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stepsize, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Stepsize
provider_slug: stepsize
slug: stepsize-domain-security
source_filename: stepsize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stepsize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 18:16:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stepsize.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/stepsize/security/stepsize-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Dashboard
- Jira
- Linear
- Software-Management
---
