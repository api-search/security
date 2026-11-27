---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 iodef "mailto:dmarc@mt-transition.fr"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mt-transition.fr
  spf: true
hosts:
- cert_expires: Jan  7 13:15:01 2027 GMT
  host: mt-transition.fr
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MT-Transition Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MT-Transition, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MT-Transition
provider_slug: mt-transition-fr
slug: mt-transition-fr-domain-security
source_filename: mt-transition-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mt-transition.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 13:15:01 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: mt-transition.fr\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:dmarc@mt-transition.fr\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mt-transition-fr/security/mt-transition-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Management
- Transition
- Industrial
- Consulting
---
