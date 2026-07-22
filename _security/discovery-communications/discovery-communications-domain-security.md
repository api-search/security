---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wbd.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: discovery-communications.com
  spf: false
hosts:
- cert_expires: Aug 10 17:31:01 2026 GMT
  host: www.wbd.com
  hsts: true
  hsts_max_age: 60
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 14:02:26 2026 GMT
  host: www.discovery-communications.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Discovery Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Discovery Communications, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Discovery Communications
provider_slug: discovery-communications
slug: discovery-communications-domain-security
source_filename: discovery-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wbd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 17:31:01 2026 GMT\n  hsts: true\n  hsts_max_age: 60\n- host: www.discovery-communications.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 14:02:26 2026 GMT\n  hsts: false\ndomains:\n- domain: wbd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: discovery-communications.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discovery-communications/refs/heads/main/security/discovery-communications-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Media
- Entertainment
- Television
- Streaming
- Fortune 500
---
