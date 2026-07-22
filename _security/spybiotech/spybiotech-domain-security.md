---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spybiotech.com
  spf: true
hosts:
- cert_expires: Sep 14 10:51:06 2026 GMT
  host: spybiotech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spybiotech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpyBiotech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SpyBiotech
provider_slug: spybiotech
slug: spybiotech-domain-security
source_filename: spybiotech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spybiotech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 10:51:06 2026 GMT\n  hsts: false\ndomains:\n- domain: spybiotech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spybiotech/refs/heads/main/security/spybiotech-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Life Sciences
- Biotechnology
- Vaccines
- Immunology
- Pharmaceuticals
- Drug Development
---
