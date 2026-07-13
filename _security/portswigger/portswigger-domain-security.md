---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:sysops@portswigger.net"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: portswigger.net
  spf: true
hosts:
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: portswigger.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Portswigger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PortSwigger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PortSwigger
provider_slug: portswigger
slug: portswigger-domain-security
source_filename: portswigger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portswigger.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: portswigger.net\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:sysops@portswigger.net\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portswigger/refs/heads/main/security/portswigger-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Security
- Web Security
- Penetration Testing
- DAST
- API Security
- Developer Tools
---
