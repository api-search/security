---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ferrellgas.com
  spf: true
  spf_record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com -all
hosts:
- cert_expires: Nov 29 22:09:07 2026 GMT
  host: www.ferrellgas.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ferrellgas Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ferrellgas Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ferrellgas Partners
provider_slug: ferrellgas-partners
slug: ferrellgas-partners-domain-security
source_filename: ferrellgas-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ferrellgas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 22:09:07 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: ferrellgas.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com -all\n  dmarc: true\n  dmarc_policy: reject\nx-probe-notes:\n- >-\n  SPF corrected by hand after verification. ferrellgas.com publishes seven TXT records, and the\n  answer exceeds what a single UDP query returns here, so the shared probe's\n  `dig +short +time=2 +tries=1 TXT` call times out and records spf: false. Re-queried three\n  times over UDP (all timed out, rc=9) and once with `dig +short +tcp TXT ferrellgas.com`,\n  which returns \"v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com -all\". The SPF record is\n  present; the false is a probe artifact, not a provider gap.\n\
  - >-\n  Mail is on Proofpoint Email Protection — the SPF record uses the pphosted.com macro form and\n  _dmarc.ferrellgas.com is CNAME'd to _dmarc.ferrellgas.com.dmarc.has.pphosted.com, which\n  answers p=reject with Proofpoint rua/ruf addresses.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ferrellgas-partners/refs/heads/main/security/ferrellgas-partners-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Propane
- Distribution
- Fuel
- Logistics
- Retail
- Utilities
- Company
---
