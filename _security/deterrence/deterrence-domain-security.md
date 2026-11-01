---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: deterrence.com
  spf: true
hosts:
- cert_expires: Apr 25 23:59:59 2027 GMT
  host: deterrence.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deterrence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deterrence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Deterrence
provider_slug: deterrence
slug: deterrence-domain-security
source_filename: deterrence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deterrence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: deterrence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/deterrence/security/deterrence-domain-security.yml
summary_line: TLSv1.3
tags:
- Security
- Defense
- Manufacturing
- Artificial Intelligence
- Automation
---
