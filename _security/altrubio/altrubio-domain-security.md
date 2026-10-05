---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: altrubio.com
  spf: true
hosts:
- cert_expires: Nov 25 10:13:57 2026 GMT
  host: www.altrubio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Altrubio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AltruBio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AltruBio
provider_slug: altrubio
slug: altrubio-domain-security
source_filename: altrubio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.altrubio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 10:13:57 2026 GMT\n  hsts: false\ndomains:\n- domain: altrubio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altrubio/refs/heads/main/security/altrubio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
