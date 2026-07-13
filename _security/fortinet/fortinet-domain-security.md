---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fortinet.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: www.fortinet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.fortinet.com
  https: false
- host: api.fortinet.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fortinet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortinet, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fortinet
provider_slug: fortinet
slug: fortinet-domain-security
source_filename: fortinet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fortinet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.fortinet.com\n  https: false\n- host: api.fortinet.com\n  https: false\ndomains:\n- domain: fortinet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortinet/refs/heads/main/security/fortinet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- Networking
---
