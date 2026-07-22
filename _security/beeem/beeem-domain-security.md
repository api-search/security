---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tinypost.co
  spf: true
hosts:
- cert_expires: Oct 14 21:59:49 2026 GMT
  host: tinypost.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beeem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beeem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Beeem
provider_slug: beeem
slug: beeem-domain-security
source_filename: beeem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tinypost.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:59:49 2026 GMT\n  hsts: false\ndomains:\n- domain: tinypost.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beeem/refs/heads/main/security/beeem-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
