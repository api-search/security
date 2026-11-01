---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mega.nz
  spf: true
hosts:
- cert_expires: Jan  7 22:00:55 2027 GMT
  host: mega.nz
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mega Nz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MEGA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MEGA
provider_slug: mega-nz
slug: mega-nz-domain-security
source_filename: mega-nz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mega.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 22:00:55 2027 GMT\n  hsts: null\ndomains:\n- domain: mega.nz\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mega-nz/security/mega-nz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
