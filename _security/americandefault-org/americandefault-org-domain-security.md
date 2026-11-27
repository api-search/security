---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: americandefault.org
  spf: true
hosts:
- cert_expires: Jan 12 00:57:38 2027 GMT
  host: americandefault.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: American Default Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Default Research, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: American Default Research
provider_slug: americandefault-org
slug: americandefault-org-domain-security
source_filename: americandefault-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: americandefault.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 00:57:38 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: americandefault.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/americandefault-org/security/americandefault-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Data
- Research
- Economics
- US
---
