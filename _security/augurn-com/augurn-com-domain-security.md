---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: augurn.com
  spf: true
hosts:
- cert_expires: Dec 15 11:44:35 2026 GMT
  host: augurn.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Augurn Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for augurn-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: augurn-com
provider_slug: augurn-com
slug: augurn-com-domain-security
source_filename: augurn-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: augurn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 11:44:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: augurn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/augurn-com/security/augurn-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
