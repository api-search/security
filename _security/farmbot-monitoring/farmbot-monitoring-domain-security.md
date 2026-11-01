---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: farmbot.com.au
  spf: true
hosts:
- cert_expires: Dec 30 01:12:31 2026 GMT
  host: farmbot.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Farmbot Monitoring Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farmbot Monitoring Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Farmbot Monitoring Solutions
provider_slug: farmbot-monitoring
slug: farmbot-monitoring-domain-security
source_filename: farmbot-monitoring-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: farmbot.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 01:12:31 2026 GMT\n  hsts: false\ndomains:\n- domain: farmbot.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/farmbot-monitoring/security/farmbot-monitoring-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AgTech
- Water Monitoring
- Sensors
- Australia
- Farm Management
---
