---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: hpcontrol.pl
  spf: true
hosts:
- cert_expires: Jan 18 08:34:06 2027 GMT
  host: hpcontrol.pl
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: hpcontrol-pl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hpcontrol-pl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: hpcontrol-pl
provider_slug: hpcontrol-pl
slug: hpcontrol-pl-domain-security
source_filename: hpcontrol-pl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hpcontrol.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 08:34:06 2027 GMT\n  hsts: null\ndomains:\n- domain: hpcontrol.pl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hpcontrol-pl/security/hpcontrol-pl-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
