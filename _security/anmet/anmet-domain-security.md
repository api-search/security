---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: anmet.com.pl
  spf: true
hosts:
- cert_expires: Nov 24 00:00:00 2026 GMT
  host: www.anmet.com.pl
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anmet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anmet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Anmet
provider_slug: anmet
slug: anmet-domain-security
source_filename: anmet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anmet.com.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 00:00:00 2026 GMT\n  hsts: false\ndomains:\n- domain: anmet.com.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anmet/refs/heads/main/security/anmet-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
