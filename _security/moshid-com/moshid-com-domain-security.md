---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moshid.com
  spf: true
hosts:
- cert_expires: Dec 28 23:10:23 2026 GMT
  host: moshid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Moshid AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moshid AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moshid AI
provider_slug: moshid-com
slug: moshid-com-domain-security
source_filename: moshid-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moshid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:10:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: moshid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/moshid-com/security/moshid-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- SEO
---
