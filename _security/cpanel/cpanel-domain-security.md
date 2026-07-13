---
api_specs:
- filename: cpanel-openapi.yml
  format: yaml
  label: cPanel UAPI
  slug: uapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cpanel/refs/heads/main/openapi/cpanel-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "godaddy.com"
  - 0 iodef "mailto:caa-notify@cpanel.net"
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cpanel.net
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: cpanel.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:32:52 2026 GMT
  host: api.docs.cpanel.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cpanel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cPanel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: cPanel
provider_slug: cpanel
slug: cpanel-domain-security
source_filename: cpanel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cpanel.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: false\n- host: api.docs.cpanel.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:32:52 2026 GMT\n  hsts: false\ndomains:\n- domain: cpanel.net\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"godaddy.com\"\n  - 0 iodef \"mailto:caa-notify@cpanel.net\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cpanel/refs/heads/main/security/cpanel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Control Panel
- DNS
- Domains
- Email
- Hosting
- Reseller
- Server Administration
- Web Hosting
- WHM
---
