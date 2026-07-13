---
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "emsign.com"
  - 0 iodef "mailto:pki@unibe.ch"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: unibe.ch
  spf: true
hosts:
- cert_expires: Aug 16 06:37:09 2026 GMT
  host: www.unibe.ch
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 23:09:13 2026 GMT
  host: boris-portal.unibe.ch
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 06:08:51 2026 GMT
  host: www.ub.unibe.ch
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Bern Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Bern, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: University of Bern
provider_slug: university-of-bern
slug: university-of-bern-domain-security
source_filename: university-of-bern-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unibe.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 06:37:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: boris-portal.unibe.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 23:09:13 2026 GMT\n  hsts: false\n- host: www.ub.unibe.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 06:08:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: unibe.ch\n  dnssec: true\n  caa:\n  - 0 issuewild \";\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"emsign.com\"\n  - 0 iodef \"mailto:pki@unibe.ch\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-bern/refs/heads/main/security/university-of-bern-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Switzerland
- Research
- Open Access
- Institutional Repository
- Library
---
