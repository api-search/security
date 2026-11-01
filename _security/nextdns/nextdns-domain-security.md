---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issue "zerossl.com"
  dmarc: false
  dnssec: true
  domain: nextdns.io
  spf: true
hosts:
- cert_expires: Dec 21 12:38:45 2026 GMT
  host: nextdns.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 10:37:00 2027 GMT
  host: api.nextdns.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Nextdns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NextDNS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: NextDNS
provider_slug: nextdns
slug: nextdns-domain-security
source_filename: nextdns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nextdns.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 12:38:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.nextdns.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 10:37:00 2027 GMT\n  hsts: null\ndomains:\n- domain: nextdns.io\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"zerossl.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nextdns/security/nextdns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- DNS
- Security
- Privacy
- Filtering
- Analytics
---
