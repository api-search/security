---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: enfabrica.net
  spf: true
hosts:
- cert_expires: Sep 16 23:10:31 2026 GMT
  host: enfabrica.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enfabrica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enfabrica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Enfabrica
provider_slug: enfabrica
slug: enfabrica-domain-security
source_filename: enfabrica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enfabrica.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:10:31 2026 GMT\n  hsts: false\ndomains:\n- domain: enfabrica.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enfabrica/refs/heads/main/security/enfabrica-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Semiconductors
- AI Infrastructure
- Networking
- Hardware
- SuperNIC
- Memory Fabric
---
