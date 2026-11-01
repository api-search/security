---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: softsync.io
  spf: true
hosts:
- cert_expires: Jan 11 13:11:13 2027 GMT
  host: softsync.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Softsync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scopic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Scopic
provider_slug: softsync
slug: softsync-domain-security
source_filename: softsync-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: softsync.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 13:11:13 2027 GMT\n  hsts: false\ndomains:\n- domain: softsync.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/softsync/security/softsync-domain-security.yml
summary_line: TLSv1.3
tags:
- Integration
- Project Management
- Automation
- Jira
- Teamwork
---
