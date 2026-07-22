---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@evroc.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: evroc.com
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: evroc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evroc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for evroc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: evroc
provider_slug: evroc
slug: evroc-domain-security
source_filename: evroc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evroc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: evroc.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@evroc.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evroc/refs/heads/main/security/evroc-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cloud Computing
- Sovereign Cloud
- Infrastructure
- Object Storage
- Compute
- AI Infrastructure
- GPU
- Europe
- IaaS
---
