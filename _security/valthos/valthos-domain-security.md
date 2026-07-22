---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: valthos.com
  spf: true
hosts:
- cert_expires: Oct  9 22:06:37 2026 GMT
  host: valthos.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valthos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valthos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Valthos
provider_slug: valthos
slug: valthos-domain-security
source_filename: valthos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: valthos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 22:06:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: valthos.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valthos/refs/heads/main/security/valthos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defense Bio
- Biodefense
- Biosecurity
- Artificial Intelligence
- Medical Countermeasures
- Life Sciences
- National Security
- New York
---
