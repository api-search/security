---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atolls.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: dmarc_rua@atolls.com
  dnssec: false
  domain: mydealz.de
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: dmarc_rua@atolls.com
  dnssec: false
  domain: hotukdeals.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: PowerDMARC-hosted aggregate mailbox
  dmarc_subdomain_policy: quarantine
  dnssec: false
  domain: igraal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: PowerDMARC-hosted aggregate mailbox
  dmarc_subdomain_policy: none
  dnssec: false
  domain: shoop.de
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: dmarc_rua@atolls.com
  dnssec: false
  domain: coupons.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: dmarc_rua@atolls.com
  dnssec: false
  domain: pepper.com
  spf: true
hosts:
- cert_expires: Oct  8 06:32:42 2026 GMT
  host: atolls.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 16:25:09 2026 GMT
  host: www.mydealz.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 06:59:15 2026 GMT
  host: www.hotukdeals.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.igraal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 12:54:37 2026 GMT
  host: www.shoop.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:42:24 2026 GMT
  host: www.coupons.com
  hsts: true
  hsts_header: max-age=31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 05:08:48 2026 GMT
  host: www.pepper.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atolls Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atolls, probed live across 7 host(s) and 7 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Atolls
provider_slug: atolls
slug: atolls-domain-security
source_filename: atolls-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the corporate host and every Atolls-owned brand host\nnote: >-\n  Atolls publishes no API host, so the probe set is the corporate domain plus the\n  consumer brand domains it operates. Every domain enforces DMARC p=reject; none\n  publishes DNSSEC or CAA; HSTS is present only on coupons.com.\nhosts:\n- host: atolls.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 06:32:42 2026 GMT\n  hsts: false\n- host: www.mydealz.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:25:09 2026 GMT\n  hsts: false\n- host: www.hotukdeals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:59:15 2026 GMT\n  hsts: false\n- host: www.igraal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\n- host: www.shoop.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 12:54:37 2026 GMT\n  hsts: false\n- host: www.coupons.com\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:42:24 2026 GMT\n  hsts: true\n  hsts_header: max-age=31536000\n- host: www.pepper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:08:48 2026 GMT\n  hsts: false\ndomains:\n- domain: atolls.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mydealz.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: dmarc_rua@atolls.com\n- domain: hotukdeals.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: dmarc_rua@atolls.com\n- domain: igraal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_subdomain_policy: quarantine\n  dmarc_rua: PowerDMARC-hosted aggregate mailbox\n- domain: shoop.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_subdomain_policy: none\n  dmarc_rua: PowerDMARC-hosted aggregate\
  \ mailbox\n- domain: coupons.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: dmarc_rua@atolls.com\n- domain: pepper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: dmarc_rua@atolls.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atolls/refs/heads/main/security/atolls-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- E-Commerce
- Affiliate Marketing
- Cashback
- Coupons
- Shopping
- Retail
- Identity
- OpenID Connect
---
