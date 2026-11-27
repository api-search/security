---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opengroup.org
  spf: true
hosts:
- cert_expires: Apr  5 18:59:41 2027 GMT
  host: community.opengroup.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OSDU Data Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OSDU Data Platform, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OSDU Data Platform
provider_slug: opengroup-org
slug: opengroup-org-domain-security
source_filename: opengroup-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: community.opengroup.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 18:59:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: opengroup.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/opengroup-org/security/opengroup-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- OSDU
- Data Platform
- Open-Group
- Oil and Gas
- Open Source
---
