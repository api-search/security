---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: septa.org
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www3.septa.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Transport For Philadelphia Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Philadelphia, US, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Transport for Philadelphia, US
provider_slug: transport-for-philadelphia-us
slug: transport-for-philadelphia-us-domain-security
source_filename: transport-for-philadelphia-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www3.septa.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: septa.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-philadelphia-us/refs/heads/main/security/transport-for-philadelphia-us-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Transportation
- Public APIs
---
