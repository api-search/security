---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lutron.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: lutron.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lutron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lutron (Caseta), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lutron (Caseta)
provider_slug: lutron
slug: lutron-domain-security
source_filename: lutron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lutron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lutron.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lutron/security/lutron-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Lighting
- Home Automation
- Smart Home
- Energy Efficiency
---
