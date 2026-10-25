---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: storageking.com.au
  spf: true
hosts:
- cert_expires: Dec 26 16:01:01 2026 GMT
  host: www.storageking.com.au
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abacus Storage King Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abacus Storage King, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Abacus Storage King
provider_slug: abacus-storage-king
slug: abacus-storage-king-domain-security
source_filename: abacus-storage-king-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.storageking.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 16:01:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: storageking.com.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abacus-storage-king/refs/heads/main/security/abacus-storage-king-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Self Storage
- Real Estate
- REIT
- Australia
- New Zealand
- ASX Listed
---
