---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: farmneural.com
  spf: true
hosts:
- cert_expires: Jan 17 03:12:34 2027 GMT
  host: farmneural.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: farmneural-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for farmneural-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: farmneural-com
provider_slug: farmneural-com
slug: farmneural-com-domain-security
source_filename: farmneural-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: farmneural.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 03:12:34 2027 GMT\n  hsts: null\ndomains:\n- domain: farmneural.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/farmneural-com/security/farmneural-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
