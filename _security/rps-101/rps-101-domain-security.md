---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pythonanywhere.com
  spf: true
hosts:
- cert_expires: Oct  5 07:28:37 2026 GMT
  host: rps101.pythonanywhere.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rps 101 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RPS 101, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RPS 101
provider_slug: rps-101
slug: rps-101-domain-security
source_filename: rps-101-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rps101.pythonanywhere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 07:28:37 2026 GMT\n  hsts: null\ndomains:\n- domain: pythonanywhere.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rps-101/refs/heads/main/security/rps-101-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Games And Comics
- Public APIs
---
