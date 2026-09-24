---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "harica.gr"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ksat.no
  spf: true
hosts:
- cert_expires: Dec  2 12:00:07 2026 GMT
  host: ksat.no
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ksat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KSAT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: KSAT
provider_slug: ksat
slug: ksat-domain-security
source_filename: ksat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ksat.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 12:00:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ksat.no\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ksat/refs/heads/main/security/ksat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Satellite
- GroundStation
- Space
- Communications
- Norway
---
