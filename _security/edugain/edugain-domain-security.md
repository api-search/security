---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: edugain.org
  spf: true
hosts:
- cert_expires: Nov  5 08:47:39 2026 GMT
  host: edugain.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Edugain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eduGAIN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: eduGAIN
provider_slug: edugain
slug: edugain-domain-security
source_filename: edugain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edugain.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 08:47:39 2026 GMT\n  hsts: false\ndomains:\n- domain: edugain.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edugain/refs/heads/main/security/edugain-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Identity Federation
- Single Sign-On
- Education
- Research
- Access Management
---
