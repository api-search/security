---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: mysocial.io
  spf: true
hosts:
- cert_expires: Jan 31 09:51:20 2027 GMT
  host: mysocial.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mysocial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mysocial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Mysocial
provider_slug: mysocial-io
slug: mysocial-io-domain-security
source_filename: mysocial-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mysocial.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 09:51:20 2027 GMT\n  hsts: false\ndomains:\n- domain: mysocial.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mysocial-io/security/mysocial-io-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Social Media
- Analytics
- Content Intelligence
- Creator Tools
- AI Integration
---
