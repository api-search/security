---
description: ''
domains:
- caa:
  - 0 iodef "mailto:syseng@bg4team.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: biblegateway.com
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: biblegateway.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bible Gateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bible Gateway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bible Gateway
provider_slug: biblegateway
slug: biblegateway-domain-security
source_filename: biblegateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biblegateway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: biblegateway.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:syseng@bg4team.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/biblegateway/security/biblegateway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bible
- Online Scripture
- Audio Bibles
- Reading Plans
---
