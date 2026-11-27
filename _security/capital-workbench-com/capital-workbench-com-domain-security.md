---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: capital-workbench.com
  spf: true
hosts:
- cert_expires: Jan 18 05:57:31 2027 GMT
  host: capital-workbench.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capital Workbench Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capital Workbench, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Capital Workbench
provider_slug: capital-workbench-com
slug: capital-workbench-com-domain-security
source_filename: capital-workbench-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capital-workbench.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 05:57:31 2027 GMT\n  hsts: false\ndomains:\n- domain: capital-workbench.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/capital-workbench-com/security/capital-workbench-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Analytics
- Public Companies
- Data
- Platform
---
