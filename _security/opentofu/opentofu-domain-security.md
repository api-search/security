---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opentofu.org
  spf: false
hosts:
- cert_expires: Sep 15 11:40:12 2026 GMT
  host: opentofu.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opentofu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenTofu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenTofu
provider_slug: opentofu
slug: opentofu-domain-security
source_filename: opentofu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opentofu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 11:40:12 2026 GMT\n  hsts: false\ndomains:\n- domain: opentofu.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opentofu/refs/heads/main/security/opentofu-domain-security.yml
summary_line: TLSv1.3
tags:
- Cloud
- DevOps
- Infrastructure as Code
- Open Source
---
