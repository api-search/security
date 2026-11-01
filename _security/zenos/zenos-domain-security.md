---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zenos.com
  spf: true
hosts:
- cert_expires: Jan  1 20:34:09 2027 GMT
  host: zenos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zenos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zenos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zenos
provider_slug: zenos
slug: zenos-domain-security
source_filename: zenos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zenos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 20:34:09 2027 GMT\n  hsts: false\ndomains:\n- domain: zenos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/zenos/security/zenos-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Robotics
- AI
- Industrial
- Construction
---
