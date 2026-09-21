---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sublime-systems.com
  spf: true
hosts:
- cert_expires: Nov 25 00:58:12 2026 GMT
  host: sublime-systems.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sublime Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sublime Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sublime Systems
provider_slug: sublime-systems
slug: sublime-systems-domain-security
source_filename: sublime-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sublime-systems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 00:58:12 2026 GMT\n  hsts: false\ndomains:\n- domain: sublime-systems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sublime-systems/refs/heads/main/security/sublime-systems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cement
- Construction Materials
- Climate Tech
- Decarbonization
- Manufacturing
- Electrochemistry
---
