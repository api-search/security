---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dvele.com
  spf: true
hosts:
- cert_expires: Nov 26 16:30:44 2026 GMT
  host: www.dvele.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blu Homes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blu Homes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blu Homes
provider_slug: blu-homes
slug: blu-homes-domain-security
source_filename: blu-homes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dvele.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 16:30:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dvele.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blu-homes/refs/heads/main/security/blu-homes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Modular Homes
- Sustainable Housing
- Real Estate
- Dvele
---
