---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getcore.id
  spf: true
hosts:
- cert_expires: Jan 14 07:19:41 2027 GMT
  host: getcore.id
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GetCore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetCore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GetCore
provider_slug: getcore-id
slug: getcore-id-domain-security
source_filename: getcore-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getcore.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 07:19:41 2027 GMT\n  hsts: false\ndomains:\n- domain: getcore.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getcore-id/security/getcore-id-domain-security.yml
summary_line: TLSv1.3
tags:
- AI Consulting
- Chatbots
---
