---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kleinschmidtinc.com
  spf: true
hosts:
- cert_expires: Jan 12 02:07:01 2027 GMT
  host: www.kleinschmidtinc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kleinschmidt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kleinschmidt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kleinschmidt
provider_slug: kleinschmidt
slug: kleinschmidt-domain-security
source_filename: kleinschmidt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kleinschmidtinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 02:07:01 2027 GMT\n  hsts: false\ndomains:\n- domain: kleinschmidtinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kleinschmidt/security/kleinschmidt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automation
- Industrial
- Control Systems
- Manufacturing
---
