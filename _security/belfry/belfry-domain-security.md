---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: belfrysoftware.com
  spf: true
hosts:
- cert_expires: Nov 28 06:27:38 2026 GMT
  host: www.belfrysoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Belfry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Belfry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Belfry
provider_slug: belfry
slug: belfry-domain-security
source_filename: belfry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.belfrysoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 06:27:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: belfrysoftware.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/belfry/refs/heads/main/security/belfry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Software
- Scheduling
- Payroll
- GuardManagement
---
