---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: axton.ca
  spf: true
hosts:
- cert_expires: Nov 25 10:43:20 2026 GMT
  host: axton.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axton, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Axton
provider_slug: axton
slug: axton-domain-security
source_filename: axton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axton.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 10:43:20 2026 GMT\n  hsts: false\ndomains:\n- domain: axton.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axton/refs/heads/main/security/axton-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Manufacturing
- Metal Fabrication
- Industrial Equipment
- Canada
- Engineering
---
