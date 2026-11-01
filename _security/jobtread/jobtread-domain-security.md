---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jobtread.com
  spf: true
hosts:
- cert_expires: Jan 17 06:04:34 2027 GMT
  host: jobtread.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jobtread Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JobTread, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JobTread
provider_slug: jobtread
slug: jobtread-domain-security
source_filename: jobtread-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobtread.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 06:04:34 2027 GMT\n  hsts: false\ndomains:\n- domain: jobtread.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/jobtread/security/jobtread-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Construction
- Estimating
- Project Management
- SaaS
- Finance
---
