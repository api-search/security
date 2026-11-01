---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vanshul.com
  spf: true
hosts:
- cert_expires: Jan 11 10:46:26 2027 GMT
  host: vanshul.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vanshul Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vanshul-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: vanshul-com
provider_slug: vanshul-com
slug: vanshul-com-domain-security
source_filename: vanshul-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vanshul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 10:46:26 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: vanshul.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/vanshul-com/security/vanshul-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Engineer
- AI
- Robotics
- Writing
- Technology
---
