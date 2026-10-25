---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nbnco.com.au
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: nbnco.com.au
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nbn Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NBN Co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NBN Co
provider_slug: nbn-co
slug: nbn-co-domain-security
source_filename: nbn-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nbnco.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: nbnco.com.au\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nbn-co/refs/heads/main/security/nbn-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Telecommunications
- Broadband
- Wholesale
- Australia
- Network Infrastructure
- B2B
---
