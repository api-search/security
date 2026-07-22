---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: liftopia.com
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: www.liftopia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:59:59 2025 GMT
  cert_subject: C=US, ST=California, L=Palo Alto, O=Liftopia, Inc., CN=*.liftopia.com
  host: liftopia.com
  hsts: null
  https: false
  note: apex host serves an expired certificate; www.liftopia.com is the canonical reachable host
  tls_cert_error: 'certificate verify failed: certificate has expired'
kind: domain-security
layout: security
method: probed
name: Liftopia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liftopia, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Liftopia
provider_slug: liftopia
slug: liftopia-domain-security
source_filename: liftopia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liftopia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: liftopia.com\n  https: false\n  tls_cert_error: 'certificate verify failed: certificate has expired'\n  cert_subject: C=US, ST=California, L=Palo Alto, O=Liftopia, Inc., CN=*.liftopia.com\n  cert_expires: Aug 18 23:59:59 2025 GMT\n  hsts: null\n  note: apex host serves an expired certificate; www.liftopia.com is the canonical\n    reachable host\ndomains:\n- domain: liftopia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liftopia/refs/heads/main/security/liftopia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Ecommerce
- Marketplace
- Ticketing
- Skiing
- Reservations
- Recreation
---
