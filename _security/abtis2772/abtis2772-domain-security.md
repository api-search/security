---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: abtis.co.kr
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: abtis.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abtis2772 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AbTis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AbTis
provider_slug: abtis2772
slug: abtis2772-domain-security
source_filename: abtis2772-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abtis.co.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: abtis.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abtis2772/refs/heads/main/security/abtis2772-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Antibody-Drug Conjugates
- Bioconjugation
- Drug Discovery
- Oncology
- Life Sciences
- Healthcare
- South Korea
---
