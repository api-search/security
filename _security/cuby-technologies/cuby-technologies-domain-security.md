---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cubytechnologies.com
  spf: true
hosts:
- cert_expires: Dec  8 11:02:07 2026 GMT
  host: cubytechnologies.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cuby Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cuby Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cuby Technologies
provider_slug: cuby-technologies
slug: cuby-technologies-domain-security
source_filename: cuby-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cubytechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 11:02:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cubytechnologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuby-technologies/refs/heads/main/security/cuby-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Real Estate
- Manufacturing
- Housing
---
