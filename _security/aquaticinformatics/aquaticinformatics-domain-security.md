---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aquaticinformatics.com
  spf: true
hosts:
- cert_expires: Jan 16 17:46:12 2027 GMT
  host: aquaticinformatics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aquatic Informatics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aquatic Informatics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aquatic Informatics
provider_slug: aquaticinformatics
slug: aquaticinformatics-domain-security
source_filename: aquaticinformatics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aquaticinformatics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 17:46:12 2027 GMT\n  hsts: false\ndomains:\n- domain: aquaticinformatics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aquaticinformatics/security/aquaticinformatics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Water
- Data Management
- Environmental
- Software
---
