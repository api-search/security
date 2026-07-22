---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: normalyze.ai
  spf: true
  spf_record: v=spf1 include:dc-aa8e722993._spfm.normalyze.ai include:mktomail.com include:_spf.salesforce.com ~all
hosts:
- cert_issuer: Sectigo Public Server Authentication CA OV R36
  cert_not_after: '2026-12-24'
  host: www.normalyze.ai
  hsts: false
  https: true
  redirects_to: https://www.proofpoint.com/us/normalyze-is-now-proofpoint
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Normalyze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Normalyze, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Normalyze
provider_slug: normalyze
slug: normalyze-domain-security
source_filename: normalyze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig + openssl TLS/HTTP probe of normalyze.ai (2026-07-20)\nnote: >-\n  normalyze.ai (www) now issues a 301 redirect to\n  https://www.proofpoint.com/us/normalyze-is-now-proofpoint — Normalyze was\n  acquired by Proofpoint and its standalone site is a redirect/marketing\n  property. DNS-level records below are genuine for the normalyze.ai domain;\n  host-level HTTP/TLS reflects the redirect endpoint.\nhosts:\n  - host: www.normalyze.ai\n    https: true\n    tls_version: TLSv1.3\n    cert_issuer: Sectigo Public Server Authentication CA OV R36\n    cert_not_after: '2026-12-24'\n    hsts: false\n    redirects_to: https://www.proofpoint.com/us/normalyze-is-now-proofpoint\ndomains:\n  - domain: normalyze.ai\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: \"v=spf1 include:dc-aa8e722993._spfm.normalyze.ai include:mktomail.com include:_spf.salesforce.com ~all\"\n    dmarc: true\n    dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/normalyze/refs/heads/main/security/normalyze-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Data Security
- DSPM
- Data Security Posture Management
- Cloud Security
- Data Governance
- Compliance
---
