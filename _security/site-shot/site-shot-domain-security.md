---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: site-shot.com
  spf: true
hosts:
- cert_expires: Dec 31 05:28:58 2026 GMT
  host: www.site-shot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Site Shot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Site-Shot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Site-Shot
provider_slug: site-shot
slug: site-shot-domain-security
source_filename: site-shot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.site-shot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 05:28:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: site-shot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/site-shot/security/site-shot-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Screenshot
- API
- Automation
- Web
---
