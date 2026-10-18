---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dspace.org
  spf: true
hosts:
- cert_expires: Nov 24 11:07:20 2026 GMT
  host: dspace.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DSpace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DSpace
provider_slug: dspace
slug: dspace-domain-security
source_filename: dspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dspace.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 11:07:20 2026 GMT\n  hsts: false\ndomains:\n- domain: dspace.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dspace/refs/heads/main/security/dspace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Open Source
- DigitalRepository
- Academic
- Community
---
