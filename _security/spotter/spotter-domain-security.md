---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spotter.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spotterstudio.com
  note: DMARC rua reports route to dmarc@spotter.la, the corporate domain.
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spotter.la
  note: Corporate domain behind Spotter (privacy policy on www.spotter.com links to spotter.la/privacy-policy); www.spotter.la redirects to www.spotter.com.
  spf: true
hosts:
- cert_expires: Sep 29 22:43:04 2026 GMT
  host: www.spotter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 18:30:29 2026 GMT
  host: www.spotterstudio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Spotter Studio marketing site (Webflow behind Cloudflare)
  tls_version: TLSv1.3
- cert_expires: Oct 18 00:21:54 2026 GMT
  host: app.spotterstudio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Spotter Studio single-page application
  tls_version: TLSv1.3
- host: help.spotterstudio.com
  hsts: null
  https: unknown
  note: Intercom-hosted help center (CNAME us.intercomhelpcenter.com). The edge refused the TLS handshake from both LibreSSL 3.3.6 and Python/OpenSSL clients (SSLV3_ALERT_HANDSHAKE_FAILURE), so no posture could be recorded. Reachable in a browser; recorded as unknown rather than as a failure.
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Spotter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spotter, probed live across 4 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spotter
provider_slug: spotter
slug: spotter-domain-security
source_filename: spotter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + product hosts\nhosts:\n- host: www.spotter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:43:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.spotterstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 18:30:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: Spotter Studio marketing site (Webflow behind Cloudflare)\n- host: app.spotterstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 00:21:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: Spotter Studio single-page application\n- host: help.spotterstudio.com\n  https: unknown\n  tls_version: null\n  hsts: null\n  note: >-\n    Intercom-hosted help center (CNAME us.intercomhelpcenter.com). The edge refused the\n    TLS handshake from both LibreSSL 3.3.6 and Python/OpenSSL clients\n    (SSLV3_ALERT_HANDSHAKE_FAILURE), so no posture could\
  \ be recorded. Reachable in a\n    browser; recorded as unknown rather than as a failure.\ndomains:\n- domain: spotter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: spotterstudio.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n  note: DMARC rua reports route to dmarc@spotter.la, the corporate domain.\n- domain: spotter.la\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  note: >-\n    Corporate domain behind Spotter (privacy policy on www.spotter.com links to\n    spotter.la/privacy-policy); www.spotter.la redirects to www.spotter.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotter/refs/heads/main/security/spotter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Creator Economy
- Media
- YouTube
- Video
- Marketing
- Content
- Creators
- Artificial Intelligence
---
