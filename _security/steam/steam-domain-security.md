---
description: ''
domains:
- caa:
  - 0 iodef "mailto:ssl-abuse@valvesoftware.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: steampowered.com
  spf: true
- caa:
  - 0 iodef "mailto:ssl-abuse@valvesoftware.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: steam-api.com
  spf: true
hosts:
- cert_expires: Aug 17 23:59:59 2026 GMT
  host: store.steampowered.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: api.steampowered.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 31 23:59:59 2026 GMT
  host: partner.steam-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Steam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Steam, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Steam
provider_slug: steam
slug: steam-domain-security
source_filename: steam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: store.steampowered.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.steampowered.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: null\n- host: partner.steam-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: steampowered.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:ssl-abuse@valvesoftware.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: steam-api.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:ssl-abuse@valvesoftware.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steam/refs/heads/main/security/steam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gaming
- Valve
- Distribution
- Steamworks
- Marketplace
- Web API
---
