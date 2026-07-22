---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: pearlbio.com
  spf: true
hosts:
- cert_expires: Aug 25 12:49:11 2026 GMT
  host: pearlbio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pearlbio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pearlbio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Pearlbio
provider_slug: pearlbio
slug: pearlbio-domain-security
source_filename: pearlbio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pearlbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 12:49:11 2026 GMT\n  hsts: false\ndomains:\n- domain: pearlbio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pearlbio/refs/heads/main/security/pearlbio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Synthetic Biology
- Biotechnology
- Biologics
- Genome Engineering
- Ribosome Engineering
- Biomaterials
- Drug Discovery
---
