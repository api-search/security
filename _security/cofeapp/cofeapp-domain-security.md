---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cofeapp.com
  spf: true
hosts:
- cert_expires: Nov 28 18:06:34 2026 GMT
  host: www.cofeapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cofeapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cofeapp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cofeapp
provider_slug: cofeapp
slug: cofeapp-domain-security
source_filename: cofeapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cofeapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 18:06:34 2026 GMT\n  hsts: false\ndomains:\n- domain: cofeapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cofeapp/refs/heads/main/security/cofeapp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Platform
- Artificial Intelligence
- Commerce
- Procurement
- MENA
---
