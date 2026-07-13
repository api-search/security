---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arc.gov
  spf: true
hosts:
- cert_expires: Sep 30 02:01:05 2026 GMT
  host: data.arc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appalachian Regional Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appalachian Regional Commission, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Appalachian Regional Commission
provider_slug: appalachian-regional-commission
slug: appalachian-regional-commission-domain-security
source_filename: appalachian-regional-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.arc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 02:01:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arc.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/security/appalachian-regional-commission-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Appalachia
- Economic Development
- Federal Government
- Government
- Infrastructure
- Regional Development
- Workforce Development
---
