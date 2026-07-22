---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: justos.com.br
  spf: true
hosts:
- cert_expires: Oct  1 08:10:44 2026 GMT
  host: www.justos.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Justos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Justos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Justos
provider_slug: justos
slug: justos-domain-security
source_filename: justos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.justos.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:10:44 2026 GMT\n  hsts: null\ndomains:\n- domain: justos.com.br\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justos/refs/heads/main/security/justos-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurtech
- Insurance
- Auto Insurance
- Telematics
- Usage-Based Insurance
- Brazil
- MGA
---
