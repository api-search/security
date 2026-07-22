---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lydia-app.com
  spf: true
hosts:
- cert_expires: Aug 15 23:04:57 2026 GMT
  host: lydia-app.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lydia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lydia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lydia
provider_slug: lydia
slug: lydia-domain-security
source_filename: lydia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lydia-app.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 23:04:57 2026 GMT\n  hsts: false\ndomains:\n- domain: lydia-app.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lydia/refs/heads/main/security/lydia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Fintech
- Mobile Payments
- Peer-to-Peer
- Banking
- Neobank
- France
---
