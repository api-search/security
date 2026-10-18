---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: olareg.org
  spf: true
hosts:
- cert_expires: Dec 13 08:03:47 2026 GMT
  host: olareg.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Olareg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for olareg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: olareg
provider_slug: olareg
slug: olareg-domain-security
source_filename: olareg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: olareg.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 08:03:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: olareg.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olareg/refs/heads/main/security/olareg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Container Registry
- OCI
- Open Source
---
