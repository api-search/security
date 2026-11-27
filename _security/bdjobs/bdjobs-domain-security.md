---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bdjobs.com
  spf: true
hosts:
- cert_expires: Jan 13 02:25:15 2027 GMT
  host: bdjobs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BDJobs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BDJobs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BDJobs
provider_slug: bdjobs
slug: bdjobs-domain-security
source_filename: bdjobs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bdjobs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 02:25:15 2027 GMT\n  hsts: false\ndomains:\n- domain: bdjobs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bdjobs/security/bdjobs-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
