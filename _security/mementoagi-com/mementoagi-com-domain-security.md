---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mementoagi.com
  spf: true
hosts:
- cert_expires: Jan 22 16:49:36 2027 GMT
  host: mementoagi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Memento Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memento, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Memento
provider_slug: mementoagi-com
slug: mementoagi-com-domain-security
source_filename: mementoagi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mementoagi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 16:49:36 2027 GMT\n  hsts: false\ndomains:\n- domain: mementoagi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mementoagi-com/security/mementoagi-com-domain-security.yml
summary_line: TLSv1.3
tags:
- AI Memory
- Cloud dashboard
---
