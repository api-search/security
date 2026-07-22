---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: illuminem.com
  spf: true
hosts:
- cert_expires: Oct  8 04:08:13 2026 GMT
  host: illuminem.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Illuminem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for illuminem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: illuminem
provider_slug: illuminem
slug: illuminem-domain-security
source_filename: illuminem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: illuminem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:08:13 2026 GMT\n  hsts: null\ndomains:\n- domain: illuminem.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/illuminem/refs/heads/main/security/illuminem-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sustainability
- ESG
- Climate
- Energy Transition
- Data
- Media
---
