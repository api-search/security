---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tomba.io
  spf: true
hosts:
- cert_expires: Aug 31 11:00:46 2026 GMT
  host: tomba.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tomba Email Finder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tomba email finder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tomba email finder
provider_slug: tomba-email-finder
slug: tomba-email-finder-domain-security
source_filename: tomba-email-finder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tomba.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 11:00:46 2026 GMT\n  hsts: false\ndomains:\n- domain: tomba.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tomba-email-finder/refs/heads/main/security/tomba-email-finder-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Business
- Public APIs
---
