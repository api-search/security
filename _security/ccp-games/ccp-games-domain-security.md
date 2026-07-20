---
api_specs:
- filename: ccp-games-esi-openapi-original.json
  format: json
  label: EVE Swagger Interface (ESI)
  slug: eve-swagger-interface-esi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ccp-games/refs/heads/main/openapi/ccp-games-esi-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "entrust.net"
  - 0 issuewild "godaddy.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eveonline.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: false
  dnssec: false
  domain: evetech.net
  spf: false
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: developers.eveonline.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: esi.evetech.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ccp Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CCP Games, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CCP Games
provider_slug: ccp-games
slug: ccp-games-domain-security
source_filename: ccp-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.eveonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\n- host: esi.evetech.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: eveonline.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"entrust.net\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: evetech.net\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ccp-games/refs/heads/main/security/ccp-games-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Games
- MMO
- EVE Online
- Developer Platform
- OAuth
- OpenID Connect
- Player Data
- Virtual Economy
---
