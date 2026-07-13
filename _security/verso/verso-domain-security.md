---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: billerud.com
  spf: true
hosts:
- cert_expires: Feb 25 12:46:48 2027 GMT
  host: www.billerud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verso Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Verso Corporation
provider_slug: verso
slug: verso-domain-security
source_filename: verso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.billerud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 12:46:48 2027 GMT\n  hsts: false\ndomains:\n- domain: billerud.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verso/refs/heads/main/security/verso-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Paper
- Coated Paper
- Specialty Paper
- Pulp
- Manufacturing
- Publishing
- Packaging
---
