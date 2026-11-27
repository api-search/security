---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: namandu.org
  spf: false
hosts:
- cert_expires: Jan 24 04:06:39 2027 GMT
  host: namandu.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Namandu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Namandu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Namandu
provider_slug: namandu-org
slug: namandu-org-domain-security
source_filename: namandu-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: namandu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 04:06:39 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: namandu.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/namandu-org/security/namandu-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mental Health
- Artificial Intelligence
- Anonymous
- Free
- Brazil
---
