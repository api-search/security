---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dnascript.com
  spf: true
hosts:
- cert_expires: Oct 16 12:00:54 2026 GMT
  host: www.dnascript.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: syntax.dnascript.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dna Script Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DNA Script, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DNA Script
provider_slug: dna-script
slug: dna-script-domain-security
source_filename: dna-script-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dnascript.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 12:00:54 2026 GMT\n  hsts: null\n- host: syntax.dnascript.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dnascript.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dna-script/refs/heads/main/security/dna-script-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Synthetic Biology
- Life Sciences
- DNA Synthesis
- Laboratory Instruments
- Genomics
- Scientific Computing
- GraphQL
---
