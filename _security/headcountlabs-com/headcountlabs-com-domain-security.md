---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: headcountlabs.com
  spf: true
hosts:
- cert_expires: Jan 16 00:19:27 2027 GMT
  host: headcountlabs.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Headcount Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Headcount Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Headcount Labs
provider_slug: headcountlabs-com
slug: headcountlabs-com-domain-security
source_filename: headcountlabs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: headcountlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 00:19:27 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: headcountlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/headcountlabs-com/security/headcountlabs-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Job
- Data
- Recruiting
- Employment
---
