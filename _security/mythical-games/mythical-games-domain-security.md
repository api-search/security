---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mythicalgames.com
  spf: true
hosts:
- cert_expires: Oct 10 03:33:01 2026 GMT
  host: mythicalgames.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 19:53:26 2026 GMT
  host: api.mythicalgames.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mythical Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mythical Games, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Mythical Games
provider_slug: mythical-games
slug: mythical-games-domain-security
source_filename: mythical-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mythicalgames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 03:33:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mythicalgames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 19:53:26 2026 GMT\n  hsts: null\ndomains:\n- domain: mythicalgames.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mythical-games/refs/heads/main/security/mythical-games-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Gaming
- Web3
- Blockchain
- Digital Assets
- NFT
- Marketplace
- gRPC
- SDK
- Game Platform
---
