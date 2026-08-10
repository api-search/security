---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hopskipdrive.com
  spf: true
hosts:
- cert_expires: Oct 24 19:03:47 2026 GMT
  host: www.hopskipdrive.com
  hsts: null
  https: true
  note: marketing site (Next.js); no Strict-Transport-Security header observed
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: api.hopskipdrive.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 7776000
  https: true
  note: private RideIQ/app backend API host; every unauthenticated path probed returned 404
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: rideiq.hopskipdrive.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 7776000
  https: true
  note: RideIQ single-page web application (account-gated)
  server: nginx
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: events.hopskipdrive.com
  hsts: null
  https: true
  note: WebSocket event stream host (wss://events.hopskipdrive.com/ws/sub)
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: status.hopskipdrive.com
  hsts: null
  https: true
  note: Status.io-hosted public status page
  tls_version: TLSv1.3
- cert_expires: Sep 12 18:08:42 2026 GMT
  host: trust.hopskipdrive.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Vanta-hosted trust center
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:50:46 2026 GMT
  host: help.hopskipdrive.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 259200
  https: true
  note: Zendesk Guide help center
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hopskipdrive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HopSkipDrive, probed live across 7 host(s) and 1 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: HopSkipDrive
provider_slug: hopskipdrive
slug: hopskipdrive-domain-security
source_filename: hopskipdrive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + hosts discovered in RideIQ env-config.js\nhosts:\n- host: www.hopskipdrive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 19:03:47 2026 GMT\n  hsts: null\n  note: marketing site (Next.js); no Strict-Transport-Security header observed\n- host: api.hopskipdrive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n  hsts_include_subdomains: false\n  note: private RideIQ/app backend API host; every unauthenticated path probed returned 404\n- host: rideiq.hopskipdrive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n  hsts_include_subdomains: true\n  server: nginx\n  note: RideIQ single-page web application (account-gated)\n- host: events.hopskipdrive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59\
  \ 2026 GMT\n  hsts: null\n  note: WebSocket event stream host (wss://events.hopskipdrive.com/ws/sub)\n- host: status.hopskipdrive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\n  note: Status.io-hosted public status page\n- host: trust.hopskipdrive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 18:08:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: cloudflare\n  note: Vanta-hosted trust center\n- host: help.hopskipdrive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:50:46 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n  hsts_include_subdomains: true\n  server: cloudflare\n  note: Zendesk Guide help center\ndomains:\n- domain: hopskipdrive.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nx-evidence:\n  probed: '2026-08-04'\n  method: openssl s_client + curl -I + dig\n  notes: >-\n    Absence of a CAA record\
  \ set and absence of HSTS on www/events/status is recorded\n    as observed fact, not inferred. api./rideiq. HSTS max-age is 7776000 (90 days),\n    below the 31536000 (1 year) HSTS-preload threshold.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopskipdrive/refs/heads/main/security/hopskipdrive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Transportation
- Student Transportation
- Education
- Mobility
- Ridesharing
- School Districts
- Logistics
- Routing
- Government
---
