---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: defined.net
  spf: true
hosts:
- cert_expires: Jan 11 14:17:59 2027 GMT
  host: www.defined.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Defined Networking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defined Networking, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Defined Networking
provider_slug: defined-networking
slug: defined-networking-domain-security
source_filename: defined-networking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.defined.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 14:17:59 2027 GMT\n  hsts: false\ndomains:\n- domain: defined.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/defined-networking/security/defined-networking-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Remote access
- Encryption
- Multi‑cloud
- IoT
- NAT traversal
- Identity
- Managed networking
---
