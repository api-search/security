---
description: ''
domains:
- caa:
  - 0 iodef "mailto:caa-reports@hackerone.com"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hackerone.com
  spf: true
hosts:
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: api.hackerone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hackerone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HackerOne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: HackerOne
provider_slug: hackerone
slug: hackerone-domain-security
source_filename: hackerone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.hackerone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hackerone.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:caa-reports@hackerone.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hackerone/refs/heads/main/security/hackerone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Public APIs
---
