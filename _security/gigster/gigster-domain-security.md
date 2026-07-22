---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gigster.com
  spf: true
hosts:
- cert_expires: Jul 31 00:58:52 2026 GMT
  host: gigster.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gigster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gigster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gigster
provider_slug: gigster
slug: gigster-domain-security
source_filename: gigster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gigster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 00:58:52 2026 GMT\n  hsts: false\ndomains:\n- domain: gigster.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigster/refs/heads/main/security/gigster-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Software Development
- Managed Services
- Staff Augmentation
- Artificial Intelligence
- Talent Marketplace
- Digital Transformation
- System Modernization
---
