---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: employmentrightschecker.co.uk
  spf: true
hosts:
- cert_expires: Jan 10 02:52:08 2027 GMT
  host: employmentrightschecker.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Employment Rights Checker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Employment Rights Checker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Employment Rights Checker
provider_slug: employmentrightschecker-co-uk
slug: employmentrightschecker-co-uk-domain-security
source_filename: employmentrightschecker-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: employmentrightschecker.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 02:52:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: employmentrightschecker.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/employmentrightschecker-co-uk/security/employmentrightschecker-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Employment
- Rights
- United Kingdom
- Human Resources
- Government
---
