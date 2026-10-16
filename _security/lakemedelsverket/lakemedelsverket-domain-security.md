---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "telia.com"
  - 0 issuewild "telia.com"
  - 0 iodef "mailto:tech@mpa.se"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lakemedelsverket.se
  spf: true
hosts:
- cert_expires: Dec 16 21:29:06 2026 GMT
  host: www.lakemedelsverket.se
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lakemedelsverket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lakemedelsverket (Swedish Medical Products Agency), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lakemedelsverket (Swedish Medical Products Agency)
provider_slug: lakemedelsverket
slug: lakemedelsverket-domain-security
source_filename: lakemedelsverket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lakemedelsverket.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 21:29:06 2026 GMT\n  hsts: false\ndomains:\n- domain: lakemedelsverket.se\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"telia.com\"\n  - 0 issuewild \"telia.com\"\n  - 0 iodef \"mailto:tech@mpa.se\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakemedelsverket/refs/heads/main/security/lakemedelsverket-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Government
- Health
- Sweden
- Pharmaceuticals
- Regulation
---
