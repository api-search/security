---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getstrada.com
  spf: true
hosts:
- cert_expires: Dec 27 19:16:28 2026 GMT
  host: getstrada.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getstrada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Strada
provider_slug: getstrada
slug: getstrada-domain-security
source_filename: getstrada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getstrada.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 19:16:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getstrada.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/getstrada/security/getstrada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Insurance
- Automation
- Platform
---
