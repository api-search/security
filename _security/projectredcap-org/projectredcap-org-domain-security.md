---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: projectredcap.org
  spf: false
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: projectredcap.org
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: REDCap (Vanderbilt) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REDCap (Vanderbilt), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: REDCap (Vanderbilt)
provider_slug: projectredcap-org
slug: projectredcap-org-domain-security
source_filename: projectredcap-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: projectredcap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: projectredcap.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/projectredcap-org/security/projectredcap-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Research
- Clinical Research
- Surveys
- Data Capture
- Healthcare
- Self-Hosted
---
