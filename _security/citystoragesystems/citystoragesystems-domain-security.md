---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: city-storage.com
  spf: true
hosts:
- cert_expires: Nov  7 17:26:41 2026 GMT
  host: city-storage.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Citystoragesystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citystoragesystems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Citystoragesystems
provider_slug: citystoragesystems
slug: citystoragesystems-domain-security
source_filename: citystoragesystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: city-storage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 17:26:41 2026 GMT\n  hsts: false\ndomains:\n- domain: city-storage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citystoragesystems/refs/heads/main/security/citystoragesystems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
