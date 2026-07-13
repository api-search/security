---
api_specs:
- filename: swagger.json
  format: json
  label: EVE Swagger Interface (ESI)
  slug: eve-swagger-interface
  spec_type: OpenAPI
  url: https://esi.evetech.net/latest/swagger.json
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eveonline.com
  spf: true
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: evetech.net
  spf: false
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: www.eveonline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: developers.eveonline.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: esi.evetech.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eve Online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EVE Online, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EVE Online
provider_slug: eve-online
slug: eve-online-domain-security
source_filename: eve-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eveonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.eveonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\n- host: esi.evetech.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: eveonline.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: evetech.net\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\
  \n  - 0 issuewild \"amazonaws.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eve-online/refs/heads/main/security/eve-online-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Authorization
- Gaming
- Images
- MMO
- OAuth2
- REST
- SSO
- Static Data
---
