---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: anonos.com
  spf: true
hosts:
- cert_expires: Dec 17 06:01:19 2026 GMT
  host: anonos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anonos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anonos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Anonos
provider_slug: anonos
slug: anonos-domain-security
source_filename: anonos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anonos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 06:01:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anonos.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anonos/refs/heads/main/security/anonos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Tokenization
- Data Privacy
- Data Security
- Enterprise Data
- Analytics
- Compliance
---
