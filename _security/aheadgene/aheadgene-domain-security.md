---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aheadgene.com
  mx:
  - mxbiz1.qq.com
  - mxbiz2.qq.com
  spf: true
  spf_record: v=spf1 include:spf.mail.qq.com ~all
hosts:
- cert_expires: null
  host: aheadgene.com
  hsts: null
  https: false
  note: Apex presents a SELF-SIGNED certificate (empty subject and issuer, notBefore 2026-06-08, notAfter 2036-06-05); the TLS handshake fails verification, so https://aheadgene.com/ is unreachable to any ordinary client. Only the www host is usable.
  tls_version: null
- cert_expires: Nov  8 23:59:59 2026 GMT
  cert_issuer: TrustAsia DV TLS RSA CA 2024
  host: www.aheadgene.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Aheadgene Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AheadGene, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AheadGene
provider_slug: aheadgene
slug: aheadgene-domain-security
source_filename: aheadgene-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aheadgene.com\n  https: false\n  tls_version: null\n  cert_expires: null\n  hsts: null\n  note: >-\n    Apex presents a SELF-SIGNED certificate (empty subject and issuer, notBefore 2026-06-08,\n    notAfter 2036-06-05); the TLS handshake fails verification, so https://aheadgene.com/ is\n    unreachable to any ordinary client. Only the www host is usable.\n- host: www.aheadgene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: false\n  cert_issuer: TrustAsia DV TLS RSA CA 2024\ndomains:\n- domain: aheadgene.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  mx: [mxbiz1.qq.com, mxbiz2.qq.com]\n  spf_record: v=spf1 include:spf.mail.qq.com ~all\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aheadgene/refs/heads/main/security/aheadgene-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Synthetic Biology
- Biotechnology
- Protein Engineering
- Life Sciences
- Pharmaceuticals
- Chemicals
- China
---
