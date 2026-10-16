---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: chipletz.com
  spf: true
hosts:
- cert_expires: Dec 27 12:19:26 2026 GMT
  host: www.chipletz.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chipletz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chipletz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Chipletz
provider_slug: chipletz
slug: chipletz-domain-security
source_filename: chipletz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chipletz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 12:19:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: chipletz.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chipletz/refs/heads/main/security/chipletz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Advanced Packaging
- Semiconductor
- AI
- HPC
- Compute
- Interconnects
---
