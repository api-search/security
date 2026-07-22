---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: epiodyne.com
  spf: true
hosts:
- cert_expires: Oct 12 21:24:47 2026 GMT
  host: epiodyne.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epiodyne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epiodyne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Epiodyne
provider_slug: epiodyne
slug: epiodyne-domain-security
source_filename: epiodyne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: epiodyne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 21:24:47 2026 GMT\n  hsts: false\ndomains:\n- domain: epiodyne.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epiodyne/refs/heads/main/security/epiodyne-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Pharmaceuticals
- Biotechnology
- Drug Discovery
- Pain Management
- Opioid Use Disorder
- Life Sciences
- Healthcare
---
