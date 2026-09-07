---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: conagrabrands.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; fo=1; rua=mailto:dmarc_rua@emaildefense.proofpoint.com; ruf=mailto:dmarc_ruf@emaildefense.proofpoint.com
  dnssec: false
  domain: conagrafoods.com
  spf: true
  spf_record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com ~all
hosts:
- cert_expires: Oct 12 03:26:32 2026 GMT
  host: www.conagrabrands.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Cloudflare returns HTTP 429 / interactive challenge to non-browser clients; the HSTS header is still emitted.
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: conagrafoods.com
  hsts: null
  http_status: 301
  https: true
  note: Legacy ConAgra Foods domain; permanent redirect to the successor brand.
  redirects_to: https://conagrabrands.com/
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Conagra Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConAgra Foods, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: ConAgra Foods
provider_slug: conagra-foods
slug: conagra-foods-domain-security
source_filename: conagra-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the ConAgra Foods legacy domain and the successor Conagra Brands domain\nnote: >-\n  ConAgra Foods, Inc. renamed to Conagra Brands, Inc. in 2015. The legacy\n  conagrafoods.com domain is still registered and answers on TLS, but 301s to\n  conagrabrands.com. Both domains are probed here so the historical alias record\n  carries its own measurement rather than inheriting the successor's.\nhosts:\n- host: www.conagrabrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:26:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: Cloudflare returns HTTP 429 / interactive challenge to non-browser clients; the HSTS header is still emitted.\n- host: conagrafoods.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\n  redirects_to: https://conagrabrands.com/\n  http_status: 301\n  note: Legacy ConAgra Foods domain; permanent redirect to\
  \ the successor brand.\ndomains:\n- domain: conagrabrands.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: conagrafoods.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com ~all'\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: 'v=DMARC1; p=reject; fo=1; rua=mailto:dmarc_rua@emaildefense.proofpoint.com; ruf=mailto:dmarc_ruf@emaildefense.proofpoint.com'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conagra-foods/refs/heads/main/security/conagra-foods-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Alias
- Branded Foods
- CPG
- Consumer Packaged Goods
- Historical
- Renamed
- Fortune 500
---
