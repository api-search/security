---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: json.org
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: www.json.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Json Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JSON, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JSON
provider_slug: json
slug: json-domain-security
source_filename: json-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.json.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: json.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/json/refs/heads/main/security/json-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Format
- Serialization
- Web Development
- JSON
- RFC 8259
---
