---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: qolapps.org
  spf: true
hosts:
- cert_expires: Jan  9 11:35:34 2027 GMT
  host: qolapps.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qolapps Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for qolapps-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: qolapps-org
provider_slug: qolapps-org
slug: qolapps-org-domain-security
source_filename: qolapps-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qolapps.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 11:35:34 2027 GMT\n  hsts: false\ndomains:\n- domain: qolapps.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/qolapps-org/security/qolapps-org-domain-security.yml
summary_line: TLSv1.3
tags:
- iOS
- Android
- Privacy
- Developer
- Apps
---
