---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: citizen.com
  spf: true
hosts:
- cert_expires: Sep 26 22:35:36 2026 GMT
  host: citizen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Citizen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citizen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Citizen
provider_slug: citizen
slug: citizen-domain-security
source_filename: citizen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: citizen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:35:36 2026 GMT\n  hsts: false\ndomains:\n- domain: citizen.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citizen/refs/heads/main/security/citizen-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Public Safety
- Safety
- Mobile Application
- Location Based Services
- Real Time Alerts
- Consumer
- Emergency
---
