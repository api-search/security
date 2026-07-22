---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: exclaimer.com
  spf: true
hosts:
- cert_expires: Oct 12 03:45:51 2026 GMT
  host: exclaimer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exclaimer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exclaimer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Exclaimer
provider_slug: exclaimer
slug: exclaimer-domain-security
source_filename: exclaimer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exclaimer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:45:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: exclaimer.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exclaimer/refs/heads/main/security/exclaimer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Email
- Email Signatures
- Email Signature Management
- Microsoft 365
- Google Workspace
- Marketing
- Productivity
- SaaS
- Security
---
