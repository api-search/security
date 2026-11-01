---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: remotelock.com
  spf: true
hosts:
- cert_expires: Jan 10 22:12:57 2027 GMT
  host: remotelock.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: api.remotelock.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Remotelock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RemoteLock, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RemoteLock
provider_slug: remotelock
slug: remotelock-domain-security
source_filename: remotelock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: remotelock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 22:12:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.remotelock.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: remotelock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/remotelock/security/remotelock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Access Control
- IoT
- Smart Locks
- Property Management
- API
---
