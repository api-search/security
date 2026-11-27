---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: landed.jobs
  spf: true
hosts:
- cert_expires: Apr 14 23:59:59 2027 GMT
  host: landed.jobs
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Landed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Landed
provider_slug: landed-jobs
slug: landed-jobs-domain-security
source_filename: landed-jobs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: landed.jobs\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: landed.jobs\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/landed-jobs/security/landed-jobs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Job Search
- Automation
- Remote Work
- Startups
---
