---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lokio.org
  spf: true
hosts:
- cert_expires: Jan 30 04:16:11 2027 GMT
  host: lokio.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LOKIO Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LOKIO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LOKIO
provider_slug: lokio-org
slug: lokio-org-domain-security
source_filename: lokio-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lokio.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 04:16:11 2027 GMT\n  hsts: false\ndomains:\n- domain: lokio.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lokio-org/security/lokio-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Social
- Hyperlocal
- Community
- Real-Time
- Location-based
---
