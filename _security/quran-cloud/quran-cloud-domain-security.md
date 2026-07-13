---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: alquran.cloud
  spf: false
hosts:
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: alquran.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quran Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quran Cloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Quran Cloud
provider_slug: quran-cloud
slug: quran-cloud-domain-security
source_filename: quran-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alquran.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: alquran.cloud\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quran-cloud/refs/heads/main/security/quran-cloud-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Books
- Public APIs
---
