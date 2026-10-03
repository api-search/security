---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: branch.co
  spf: true
hosts:
- cert_expires: Dec 18 12:11:55 2026 GMT
  host: branch.co
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Branchintl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Branchintl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: Branchintl
provider_slug: branchintl
slug: branchintl-domain-security
source_filename: branchintl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: branch.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 12:11:55 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: branch.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/branchintl/refs/heads/main/security/branchintl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- fintech
- mobile
- credit
- emerging-markets
- Africa
- India
---
