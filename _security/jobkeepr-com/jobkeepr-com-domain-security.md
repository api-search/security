---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jobkeepr.com
  spf: true
hosts:
- cert_expires: Jan  4 19:58:47 2027 GMT
  host: jobkeepr.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jobkeepr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jobkeepr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jobkeepr
provider_slug: jobkeepr-com
slug: jobkeepr-com-domain-security
source_filename: jobkeepr-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobkeepr.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  4 19:58:47 2027 GMT\n  hsts: false\ndomains:\n- domain: jobkeepr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jobkeepr-com/security/jobkeepr-com-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Field Service Management
- Contractors
- Software-as-a-Service
- Scheduling
- Invoicing
---
