---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: federation.edu.au
  spf: true
hosts:
- cert_expires: Nov 28 10:15:14 2026 GMT
  host: federation.edu.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Federation University Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federation University Australia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Federation University Australia
provider_slug: federation-university-australia
slug: federation-university-australia-domain-security
source_filename: federation-university-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: federation.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 10:15:14 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: federation.edu.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/federation-university-australia/security/federation-university-australia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- University
- Australia
- HigherEducation
- CooperativeEducation
- Company
---
