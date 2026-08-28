---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ndrip.com
  spf: true
hosts:
- cert_expires: Oct 11 11:45:46 2026 GMT
  host: ndrip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: app.ndrip.com
  hsts: false
  https: true
  note: N-Drip Connect web application (S3 + CloudFront origin); added by the enrichment pass because apis[] is empty so the automated probe did not reach it.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: N Drip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for N-Drip, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: N-Drip
provider_slug: n-drip
slug: n-drip-domain-security
source_filename: n-drip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ndrip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 11:45:46 2026 GMT\n  hsts: false\n- host: app.ndrip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\n  note: N-Drip Connect web application (S3 + CloudFront origin); added by the enrichment pass because\n    apis[] is empty so the automated probe did not reach it.\ndomains:\n- domain: ndrip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnote: ndrip.com serves no HSTS header and publishes no CAA record or DNSSEC; SPF and DMARC are present\n  but DMARC policy is p=none (monitor only, no enforcement). Both company hosts negotiate TLS 1.3.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n-drip/refs/heads/main/security/n-drip-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agriculture
- AgTech
- Irrigation
- Water
- Water Conservation
- Sustainability
- Climate
- Precision Agriculture
- Sensors
- IoT
- Israel
---
