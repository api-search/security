---
description: ''
domains:
- caa:
  - 0 issue "microsoft.com"
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:ICT.Licensing@monadel.com.au"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: monadelphous.com.au
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: monadelphous.com.au
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Monadelphous Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monadelphous, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Monadelphous
provider_slug: monadelphous
slug: monadelphous-domain-security
source_filename: monadelphous-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monadelphous.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: monadelphous.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"microsoft.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:ICT.Licensing@monadel.com.au\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monadelphous/refs/heads/main/security/monadelphous-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Engineering
- Construction
- Maintenance Services
- Industrial Services
- Mining
- Energy
- Infrastructure
- Australia
---
