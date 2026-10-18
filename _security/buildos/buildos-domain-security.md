---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thebuildos.net
  spf: false
hosts:
- cert_expires: Dec 26 21:34:56 2026 GMT
  host: www.thebuildos.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buildos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buildos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Buildos
provider_slug: buildos
slug: buildos-domain-security
source_filename: buildos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thebuildos.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 21:34:56 2026 GMT\n  hsts: false\ndomains:\n- domain: thebuildos.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildos/refs/heads/main/security/buildos-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Construction
- Project Management
- Software
- Software-as-a-Service
- BuildOS
---
