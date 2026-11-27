---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gdacs.org
  spf: true
hosts:
- cert_expires: Dec 29 08:21:39 2026 GMT
  host: gdacs.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Global Disaster Awareness and Coordination System Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Global Disaster Awareness and Coordination System, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Global Disaster Awareness and Coordination System
provider_slug: gdacs-org
slug: gdacs-org-domain-security
source_filename: gdacs-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gdacs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 08:21:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gdacs.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gdacs-org/security/gdacs-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Disaster
- Alerts
- Maps
- Coordination
- UN
---
