---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: saabgroup.com
  spf: true
hosts:
- cert_expires: Jan  6 19:10:06 2027 GMT
  host: www.saabgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Saab Ab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saab AB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Saab AB
provider_slug: saab-ab
slug: saab-ab-domain-security
source_filename: saab-ab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saabgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 19:10:06 2027 GMT\n  hsts: false\ndomains:\n- domain: saabgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/saab-ab/security/saab-ab-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- defence
- land systems
- naval
- security
- government
- civil security
---
