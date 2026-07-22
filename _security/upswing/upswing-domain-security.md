---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:notify-cp@upswing.one"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: upswing.one
  spf: true
hosts:
- cert_expires: Oct 16 06:12:30 2026 GMT
  host: upswing.one
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upswing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upswing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Upswing
provider_slug: upswing
slug: upswing-domain-security
source_filename: upswing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upswing.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 06:12:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: upswing.one\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:notify-cp@upswing.one\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upswing/refs/heads/main/security/upswing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Open Finance
- Embedded Finance
- Banking
- India
- Deposits
- Lending
---
