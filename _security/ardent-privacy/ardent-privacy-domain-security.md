---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ardentprivacy.ai
  spf: true
hosts:
- cert_expires: Oct  7 01:22:00 2026 GMT
  host: www.ardentprivacy.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ardent Privacy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ardent Privacy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ardent Privacy
provider_slug: ardent-privacy
slug: ardent-privacy-domain-security
source_filename: ardent-privacy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ardentprivacy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 01:22:00 2026 GMT\n  hsts: false\ndomains:\n- domain: ardentprivacy.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ardent-privacy/refs/heads/main/security/ardent-privacy-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Privacy
- Security
- Software-as-a-Service
- Compliance
---
