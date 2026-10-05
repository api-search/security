---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getboltwise.com
  spf: true
hosts:
- cert_expires: Dec 13 04:41:36 2026 GMT
  host: getboltwise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boltwise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BoltWise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BoltWise
provider_slug: boltwise
slug: boltwise-domain-security
source_filename: boltwise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getboltwise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 04:41:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getboltwise.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boltwise/refs/heads/main/security/boltwise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Quoting
- ERP Integration
- Industrial Distribution
---
