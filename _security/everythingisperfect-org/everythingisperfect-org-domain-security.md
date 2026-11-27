---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: everythingisperfect.org
  spf: true
hosts:
- cert_expires: Jan  7 02:01:20 2027 GMT
  host: everythingisperfect.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Perfect World Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perfect World Project, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Perfect World Project
provider_slug: everythingisperfect-org
slug: everythingisperfect-org-domain-security
source_filename: everythingisperfect-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: everythingisperfect.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 02:01:20 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: everythingisperfect.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/everythingisperfect-org/security/everythingisperfect-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Civic Tech
- Transparency
- Public Data
- Community
- Open Source
---
