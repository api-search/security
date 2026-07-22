---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: globelifeinsurance.com
  spf: false
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: www.globelifeinsurance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Torchmark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Globe Life (Torchmark), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Globe Life (Torchmark)
provider_slug: torchmark
slug: torchmark-domain-security
source_filename: torchmark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.globelifeinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: globelifeinsurance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/torchmark/refs/heads/main/security/torchmark-domain-security.yml
summary_line: TLSv1.3
tags:
- Annuities
- Financial Services
- Fortune 1000
- Insurance
- Life Insurance
- Supplemental Health Insurance
---
