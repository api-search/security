---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: equityzen.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atmosphere.tv
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: equityzen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: www.atmosphere.tv
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Atmospheretv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atmospheretv, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Atmospheretv
provider_slug: atmospheretv
slug: atmospheretv-domain-security
source_filename: atmospheretv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: equityzen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\n- host: www.atmosphere.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: equityzen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: atmosphere.tv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atmospheretv/refs/heads/main/security/atmospheretv-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video
- Streaming
- Advertising
- Software-as-a-Service
- Platform
---
