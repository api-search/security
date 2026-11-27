---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: terramcp.earth
  spf: false
hosts:
- cert_expires: Jan 13 15:30:00 2027 GMT
  host: terramcp.earth
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: terramcp-earth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for terramcp-earth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: terramcp-earth
provider_slug: terramcp-earth
slug: terramcp-earth-domain-security
source_filename: terramcp-earth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: terramcp.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 15:30:00 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: terramcp.earth\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/terramcp-earth/security/terramcp-earth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
