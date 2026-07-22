---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 issue "comodo.com"
  - 0 iodef "mailto:domainmaster@gamigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trionworlds.com
  spf: true
hosts:
- cert_expires: Aug 17 22:52:04 2026 GMT
  host: www.trionworlds.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trion Worlds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trion Worlds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trion Worlds
provider_slug: trion-worlds
slug: trion-worlds-domain-security
source_filename: trion-worlds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trionworlds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 22:52:04 2026 GMT\n  hsts: null\ndomains:\n- domain: trionworlds.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 issue \"comodo.com\"\n  - 0 iodef \"mailto:domainmaster@gamigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trion-worlds/refs/heads/main/security/trion-worlds-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Games
- Video Games
- MMO
- Online Games
- Entertainment
---
