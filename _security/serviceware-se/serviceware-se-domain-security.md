---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: serviceware-se.com
  spf: true
hosts:
- cert_expires: Aug 22 05:16:41 2026 GMT
  host: serviceware-se.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Serviceware Se Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Serviceware SE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Serviceware SE
provider_slug: serviceware-se
slug: serviceware-se-domain-security
source_filename: serviceware-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: serviceware-se.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 05:16:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: serviceware-se.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serviceware-se/refs/heads/main/security/serviceware-se-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Service Management
- IT Financial Management
- Corporate Performance Management
- Knowledge Management
- Field Service Management
- Enterprise Software
- Germany
---
