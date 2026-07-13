---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: resware.com
  spf: true
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qualia.com
  spf: true
hosts:
- cert_expires: Sep 13 11:50:22 2026 GMT
  host: resware.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 17:15:27 2026 GMT
  host: www.qualia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Resware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ResWare, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ResWare
provider_slug: resware
slug: resware-domain-security
source_filename: resware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: resware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 11:50:22 2026 GMT\n  hsts: null\n- host: www.qualia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:15:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: resware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: qualia.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resware/refs/heads/main/security/resware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Title
- Escrow
- Real Estate
- Closing
- Title Production
- SOAP
- XML
- WCF
- Partner API
- Gated
- Qualia
---
