---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: instapaper.com
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: instapaper.com
  hsts: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Instapaper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instapaper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Instapaper
provider_slug: instapaper
slug: instapaper-domain-security
source_filename: instapaper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instapaper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 631138519\ndomains:\n- domain: instapaper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/instapaper/security/instapaper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- read-it-later
- productivity
- web-service
- bookmarking
- API
---
