---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pgi.gov.pl
  spf: true
hosts:
- cert_expires: Dec 30 10:10:31 2026 GMT
  host: www.pgi.gov.pl
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Polish Geological Institute National Research Institute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polish Geological Institute - National Research Institute, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Polish Geological Institute - National Research Institute
provider_slug: polish-geological-institute-national-research-institute
slug: polish-geological-institute-national-research-institute-domain-security
source_filename: polish-geological-institute-national-research-institute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pgi.gov.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 10:10:31 2026 GMT\n  hsts: false\ndomains:\n- domain: pgi.gov.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/polish-geological-institute-national-research-institute/security/polish-geological-institute-national-research-institute-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geology
- Research
- Poland
- Government
---
