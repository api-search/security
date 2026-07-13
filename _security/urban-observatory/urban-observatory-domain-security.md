---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: urbanobservatory.ac.uk
  spf: false
hosts:
- cert_expires: Aug 15 02:02:12 2026 GMT
  host: urbanobservatory.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Urban Observatory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urban Observatory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Urban Observatory
provider_slug: urban-observatory
slug: urban-observatory-domain-security
source_filename: urban-observatory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urbanobservatory.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 15 02:02:12 2026 GMT\n  hsts: false\ndomains:\n- domain: urbanobservatory.ac.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urban-observatory/refs/heads/main/security/urban-observatory-domain-security.yml
summary_line: TLSv1.2
tags:
- Open Data
- Public APIs
---
