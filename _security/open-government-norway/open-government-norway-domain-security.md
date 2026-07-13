---
description: ''
domains:
- caa:
  - 0 iodef "mailto:drift@digdir.no"
  - 0 issue "pki.goog"
  - 0 issue "buypass.no"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: norge.no
  spf: true
hosts:
- cert_expires: Aug  8 21:59:00 2026 GMT
  host: data.norge.no
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Norway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Norway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Open Government, Norway
provider_slug: open-government-norway
slug: open-government-norway-domain-security
source_filename: open-government-norway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.norge.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 21:59:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: norge.no\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:drift@digdir.no\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"buypass.no\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-norway/refs/heads/main/security/open-government-norway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Public APIs
---
