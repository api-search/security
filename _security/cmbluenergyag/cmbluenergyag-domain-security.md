---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "swisssign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cmblu.com
  spf: true
hosts:
- cert_expires: Nov 14 18:33:12 2026 GMT
  host: www.cmblu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cmbluenergyag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cmbluenergyag, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cmbluenergyag
provider_slug: cmbluenergyag
slug: cmbluenergyag-domain-security
source_filename: cmbluenergyag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cmblu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 18:33:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cmblu.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"swisssign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cmbluenergyag/refs/heads/main/security/cmbluenergyag-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Battery
- Storage
- Cleantech
- Germany
- Company
---
