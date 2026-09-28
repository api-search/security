---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bioinno.com
  spf: true
hosts:
- cert_expires: Oct 11 00:02:24 2026 GMT
  host: bioinno.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bioinno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BioInno, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BioInno
provider_slug: bioinno
slug: bioinno-domain-security
source_filename: bioinno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bioinno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 00:02:24 2026 GMT\n  hsts: false\ndomains:\n- domain: bioinno.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bioinno/refs/heads/main/security/bioinno-domain-security.yml
summary_line: TLSv1.3
tags:
- Biotechnology
- Life Sciences
- Healthcare
- Research
- Company
---
