---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: securitytrails.com
  spf: true
hosts:
- cert_expires: Sep 16 14:23:07 2026 GMT
  host: securitytrails.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Securitytrails Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SecurityTrails, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SecurityTrails
provider_slug: securitytrails
slug: securitytrails-domain-security
source_filename: securitytrails-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: securitytrails.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:23:07 2026 GMT\n  hsts: null\ndomains:\n- domain: securitytrails.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securitytrails/refs/heads/main/security/securitytrails-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Security
- Public APIs
---
