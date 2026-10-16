---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alephlabs.net
  spf: false
hosts:
- cert_expires: Dec 10 20:16:32 2026 GMT
  host: alephlabs.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alephlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alephlabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Alephlabs
provider_slug: alephlabs
slug: alephlabs-domain-security
source_filename: alephlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alephlabs.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 20:16:32 2026 GMT\n  hsts: false\ndomains:\n- domain: alephlabs.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alephlabs/refs/heads/main/security/alephlabs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Software
- DeveloperTools
- Platform
- API
---
