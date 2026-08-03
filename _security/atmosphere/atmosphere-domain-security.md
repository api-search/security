---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_rua: dmarc@atmosphere.tv
  dnssec: false
  domain: atmosphere.tv
  spf: true
  spf_record: v=spf1 mx include:_spf.google.com include:spf.autopilothq.com include:21890827.spf10.hubspotemail.net ~all
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: www.atmosphere.tv
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: api.atmosphere.tv
  hsts: false
  https: true
  note: Undocumented first-party backend. GET / returns a bare version string (10.50.2) and sets an atmosphere_api_session cookie; GET /status returns {"ping":"pong","mysql":"up","redis":"up"}. Fronted by AWS API Gateway and CloudFront. No public contract is published at this host.
  tls_version: TLSv1.3
- cert_expires: Sep 30 04:10:37 2026 GMT
  host: help.atmosphere.tv
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 8 23:59:59 2027 GMT
  host: admin.atmosphere.tv
  hsts: false
  https: true
  note: Atmosphere Admin single-page console. Answers HTTP 200 with the SPA HTML shell for several /.well-known/* paths; those are catch-all responses, not published discovery documents (see well-known/atmosphere-well-known.yml).
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: advertise.atmosphere.tv
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atmosphere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atmosphere, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atmosphere
provider_slug: atmosphere
slug: atmosphere-domain-security
source_filename: atmosphere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + discovered Atmosphere subdomains\nhosts:\n- host: www.atmosphere.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\n- host: api.atmosphere.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: false\n  note: >-\n    Undocumented first-party backend. GET / returns a bare version string\n    (10.50.2) and sets an atmosphere_api_session cookie; GET /status returns\n    {\"ping\":\"pong\",\"mysql\":\"up\",\"redis\":\"up\"}. Fronted by AWS API Gateway and\n    CloudFront. No public contract is published at this host.\n- host: help.atmosphere.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:10:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: admin.atmosphere.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 8 23:59:59 2027 GMT\n  hsts: false\n  note: >-\n \
  \   Atmosphere Admin single-page console. Answers HTTP 200 with the SPA HTML\n    shell for several /.well-known/* paths; those are catch-all responses, not\n    published discovery documents (see well-known/atmosphere-well-known.yml).\n- host: advertise.atmosphere.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atmosphere.tv\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: >-\n    v=spf1 mx include:_spf.google.com include:spf.autopilothq.com\n    include:21890827.spf10.hubspotemail.net ~all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_rua: dmarc@atmosphere.tv\nfindings:\n- No CAA records published on atmosphere.tv.\n- DNSSEC not enabled on atmosphere.tv.\n- DMARC published but policy is p=none (monitor only, not enforcing).\n- HSTS present on help. and advertise. but absent on www., api. and admin.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atmosphere/refs/heads/main/security/atmosphere-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Streaming
- Television
- Advertising
- Digital Signage
- Out Of Home
- Entertainment
- Hospitality
- Connected TV
---
