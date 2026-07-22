---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: internationalpaper.com
  spf: true
hosts:
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: www.internationalpaper.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: International Paper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for International Paper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: International Paper
provider_slug: international-paper
slug: international-paper-domain-security
source_filename: international-paper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.internationalpaper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: internationalpaper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/international-paper/refs/heads/main/security/international-paper-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Fortune 500
- Manufacturing
- Packaging
- Paper
- Pulp
---
