---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hellogetsafe.com
  spf: true
hosts:
- cert_expires: Oct 13 09:47:19 2026 GMT
  host: www.hellogetsafe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getsafe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Getsafe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Getsafe
provider_slug: getsafe
slug: getsafe-domain-security
source_filename: getsafe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hellogetsafe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 09:47:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hellogetsafe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getsafe/refs/heads/main/security/getsafe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurtech
- Insurance
- Digital Insurance
- Financial Services
- Germany
- Mobile App
- Embedded Insurance
---
