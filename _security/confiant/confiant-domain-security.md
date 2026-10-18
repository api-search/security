---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: confiant.com
  spf: true
hosts:
- cert_expires: Nov 18 01:27:19 2026 GMT
  host: www.confiant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Confiant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Confiant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Confiant
provider_slug: confiant
slug: confiant-domain-security
source_filename: confiant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.confiant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 01:27:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: confiant.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confiant/refs/heads/main/security/confiant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Ad Security
- Ad Quality
- Privacy
- Publishers
- Platform
- Digital Advertising
- Malvertising
---
