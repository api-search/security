---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: knowmesh.online
  spf: false
hosts:
- cert_expires: Jan 15 06:28:31 2027 GMT
  host: knowmesh.online
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: knowmesh-online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for knowmesh-online, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: knowmesh-online
provider_slug: knowmesh-online
slug: knowmesh-online-domain-security
source_filename: knowmesh-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knowmesh.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 06:28:31 2027 GMT\n  hsts: null\ndomains:\n- domain: knowmesh.online\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/knowmesh-online/security/knowmesh-online-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
