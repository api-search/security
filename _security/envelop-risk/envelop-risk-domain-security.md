---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: enveloprisk.com
  spf: true
hosts:
- cert_expires: Oct  5 23:13:57 2026 GMT
  host: www.enveloprisk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Envelop Risk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Envelop Risk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Envelop Risk
provider_slug: envelop-risk
slug: envelop-risk-domain-security
source_filename: envelop-risk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enveloprisk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:13:57 2026 GMT\n  hsts: false\ndomains:\n- domain: enveloprisk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envelop-risk/refs/heads/main/security/envelop-risk-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Insurance
- Reinsurance
- Cyber Risk
- Underwriting
- Analytics
- Machine Learning
- Cyber Insurance
- Insurtech
---
