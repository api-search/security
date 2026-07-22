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
  dmarc_policy: quarantine
  dnssec: false
  domain: otterize.com
  spf: true
hosts:
- cert_expires: Oct  8 20:13:19 2026 GMT
  host: otterize.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Otterize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Otterize, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Otterize
provider_slug: otterize
slug: otterize-domain-security
source_filename: otterize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: otterize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 20:13:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: otterize.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/otterize/refs/heads/main/security/otterize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Business Applications
- Kubernetes
- Access Control
- Cloud Native Security
- Zero Trust
- DevSecOps
- IAM
- Open Source
---
