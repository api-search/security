---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qualia.com
  spf: true
hosts:
- cert_expires: Sep 27 17:15:27 2026 GMT
  host: www.qualia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qualia Title Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qualia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Qualia
provider_slug: qualia-title
slug: qualia-title-domain-security
source_filename: qualia-title-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qualia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:15:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qualia.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualia-title/refs/heads/main/security/qualia-title-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Title Insurance
- Escrow
- Real Estate
- Closing
- Settlement
- PropTech
- GraphQL
---
