---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: livebustimes.org
  spf: false
hosts:
- cert_expires: Jan 12 22:11:50 2027 GMT
  host: livebustimes.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Live Bus Times Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Live Bus Times, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Live Bus Times
provider_slug: livebustimes-org
slug: livebustimes-org-domain-security
source_filename: livebustimes-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: livebustimes.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 22:11:50 2027 GMT\n  hsts: false\ndomains:\n- domain: livebustimes.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/livebustimes-org/security/livebustimes-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
