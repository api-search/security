---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "zerossl.com"
  - 0 issue "zerossl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lettermint.co
  spf: true
hosts:
- cert_expires: Dec  9 18:07:20 2026 GMT
  host: lettermint.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lettermint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lettermint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lettermint
provider_slug: lettermint
slug: lettermint-domain-security
source_filename: lettermint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lettermint.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 18:07:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lettermint.co\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"zerossl.com\"\n  - 0 issue \"zerossl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lettermint/security/lettermint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Email
- Transactional
- API
- European
---
