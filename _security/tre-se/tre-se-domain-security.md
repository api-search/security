---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tre.se
  spf: true
hosts:
- cert_expires: Nov 15 11:01:04 2026 GMT
  host: tre.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tre Se Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tre (Hi3G), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tre (Hi3G)
provider_slug: tre-se
slug: tre-se-domain-security
source_filename: tre-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tre.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 11:01:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tre.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tre-se/refs/heads/main/security/tre-se-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
