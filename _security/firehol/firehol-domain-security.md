---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: firehol.org
  spf: true
hosts:
- cert_expires: Jan  2 02:53:39 2027 GMT
  host: iplists.firehol.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firehol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FireHOL IP lists, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FireHOL IP lists
provider_slug: firehol
slug: firehol-domain-security
source_filename: firehol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iplists.firehol.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 02:53:39 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: firehol.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/firehol/security/firehol-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Security
- Threat Intelligence
- IP Reputation
- IP Blocklists
- Open Source
- Firewall
- Open Data
---
