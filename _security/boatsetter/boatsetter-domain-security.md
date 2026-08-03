---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: boatsetter.com
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: www.boatsetter.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Boatsetter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boatsetter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Boatsetter
provider_slug: boatsetter
slug: boatsetter-domain-security
source_filename: boatsetter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boatsetter.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: boatsetter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boatsetter/refs/heads/main/security/boatsetter-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Boat Rental
- Peer To Peer
- Marketplace
- Travel
- Boating
- Maritime
- Yacht Charter
- Watersports
- Recreation
- Sharing Economy
---
