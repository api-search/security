---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: crazyduck.net
  spf: true
hosts:
- cert_expires: Dec 22 02:30:38 2026 GMT
  host: www.crazyduck.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crazyduck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crazyduck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Crazyduck
provider_slug: crazyduck
slug: crazyduck-domain-security
source_filename: crazyduck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crazyduck.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 02:30:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crazyduck.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crazyduck/refs/heads/main/security/crazyduck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Social
- Dating
- Adult
- Community
- Poland
---
