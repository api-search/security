---
description: ''
domains:
- caa:
  - 0 iodef "mailto:hello@fsaircraft.net"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fsaircraft.net
  spf: true
hosts:
- cert_expires: Jan  2 00:44:53 2027 GMT
  host: fsaircraft.net
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: fsaircraft-net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fsaircraft-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: fsaircraft-net
provider_slug: fsaircraft-net
slug: fsaircraft-net-domain-security
source_filename: fsaircraft-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fsaircraft.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 00:44:53 2027 GMT\n  hsts: null\ndomains:\n- domain: fsaircraft.net\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:hello@fsaircraft.net\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fsaircraft-net/security/fsaircraft-net-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
