---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: gigs.com
  spf: true
hosts:
- cert_expires: Sep 30 13:27:34 2026 GMT
  host: gigs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 12:32:24 2026 GMT
  host: developers.gigs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 11:28:39 2026 GMT
  host: api.gigs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gigs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gigs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Gigs
provider_slug: gigs
slug: gigs-domain-security
source_filename: gigs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gigs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:27:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.gigs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 12:32:24 2026 GMT\n  hsts: false\n- host: api.gigs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 11:28:39 2026 GMT\n  hsts: null\ndomains:\n- domain: gigs.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigs/refs/heads/main/security/gigs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Telecom
- Connectivity
- eSIM
- MVNO
- Mobile
- Subscriptions
- Payments
- Webhooks
- Embedded Finance
---
