---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alkane.com.au
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: alkane.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alkane Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alkane Resources, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alkane Resources
provider_slug: alkane-resources
slug: alkane-resources-domain-security
source_filename: alkane-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alkane.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: alkane.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alkane-resources/refs/heads/main/security/alkane-resources-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mining
- Gold
- Antimony
- Australia
- Natural Resources
- ASX Listed
---
