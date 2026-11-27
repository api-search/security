---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: h2-papers.org
  spf: true
hosts:
- cert_expires: Feb  6 06:25:15 2027 GMT
  host: h2-papers.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: H2 Papers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for H2 Papers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: H2 Papers
provider_slug: h2-papers-org
slug: h2-papers-org-domain-security
source_filename: h2-papers-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: h2-papers.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 06:25:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: h2-papers.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/h2-papers-org/security/h2-papers-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
---
