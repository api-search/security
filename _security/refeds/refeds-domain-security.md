---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: refeds.org
  spf: true
hosts:
- cert_expires: Nov  5 14:48:56 2026 GMT
  host: refeds.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Refeds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REFEDS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: REFEDS
provider_slug: refeds
slug: refeds-domain-security
source_filename: refeds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: refeds.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 14:48:56 2026 GMT\n  hsts: false\ndomains:\n- domain: refeds.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refeds/refs/heads/main/security/refeds-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Identity
- Federation
- Research
- Education
---
