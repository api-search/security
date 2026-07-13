---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cloudmersive.com
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: www.cloudmersive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudmersive Natural Language Processing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudmersive Natural Language Processing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cloudmersive Natural Language Processing
provider_slug: cloudmersive-natural-language-processing
slug: cloudmersive-natural-language-processing-domain-security
source_filename: cloudmersive-natural-language-processing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudmersive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cloudmersive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudmersive-natural-language-processing/refs/heads/main/security/cloudmersive-natural-language-processing-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Text Analysis
- Public APIs
---
