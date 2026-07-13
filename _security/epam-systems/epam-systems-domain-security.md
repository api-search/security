---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: epam.com
  spf: true
hosts:
- cert_expires: Sep 13 13:18:05 2026 GMT
  host: www.epam.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.epam.com
  https: false
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: api.epam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epam Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EPAM Systems, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: EPAM Systems
provider_slug: epam-systems
slug: epam-systems-domain-security
source_filename: epam-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 13:18:05 2026 GMT\n  hsts: null\n- host: developer.epam.com\n  https: false\n- host: api.epam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: epam.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epam-systems/refs/heads/main/security/epam-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Software Engineering
- Digital Transformation
---
