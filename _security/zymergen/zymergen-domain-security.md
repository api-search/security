---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: zymergen.com
  spf: true
hosts:
- cert_expires: Oct 18 16:49:24 2026 GMT
  host: zymergen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zymergen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zymergen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Zymergen
provider_slug: zymergen
slug: zymergen-domain-security
source_filename: zymergen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zymergen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 16:49:24 2026 GMT\n  hsts: null\ndomains:\n- domain: zymergen.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zymergen/refs/heads/main/security/zymergen-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Synthetic Biology
- Biotechnology
- Bio-manufacturing
- Materials Science
- Machine Learning
- Acquired
---
