---
description: ''
domains:
- caa:
  - 0 iodef "mailto:pki@libertyglobal.com"
  - 0 issue "globalsign.com"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: virginmediao2.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: virginmediao2business.co.uk
  spf: true
hosts:
- cert_expires: Dec  2 11:35:32 2026 GMT
  host: www.virginmediao2.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  3 09:11:52 2027 GMT
  host: www.virginmediao2business.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: www.o2.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virgin Media O2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virgin Media O2, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Virgin Media O2
provider_slug: virgin-media-o2
slug: virgin-media-o2-domain-security
source_filename: virgin-media-o2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.virginmediao2.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 11:35:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.virginmediao2business.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  3 09:11:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.o2.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: virginmediao2.co.uk\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:pki@libertyglobal.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: virginmediao2business.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virgin-media-o2/refs/heads/main/security/virgin-media-o2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- United Kingdom
- Mobile Network Operator
- Broadband
- Network APIs
- CAMARA
- Open Gateway
- Identity Verification
- SIM Swap
- Age Verification
- Converged Operator
- Partner Gated
---
