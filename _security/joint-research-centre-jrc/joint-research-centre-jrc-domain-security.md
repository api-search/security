---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: europa.eu
  spf: true
hosts:
- cert_expires: Feb 15 08:31:04 2027 GMT
  host: ec.europa.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Joint Research Centre Jrc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joint Research Centre (JRC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Joint Research Centre (JRC)
provider_slug: joint-research-centre-jrc
slug: joint-research-centre-jrc-domain-security
source_filename: joint-research-centre-jrc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ec.europa.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 08:31:04 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: europa.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/joint-research-centre-jrc/security/joint-research-centre-jrc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
---
