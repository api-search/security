---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: osv.dev
  spf: false
hosts:
- cert_expires: Feb  4 16:46:47 2027 GMT
  host: osv.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OSV Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OSV, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OSV
provider_slug: osv-dev
slug: osv-dev-domain-security
source_filename: osv-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: osv.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 16:46:47 2027 GMT\n  hsts: false\ndomains:\n- domain: osv.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/osv-dev/security/osv-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Vulnerability Database
- Open Source
- Scanner
- Remediation
- CI/CD
- Container Scanning
---
