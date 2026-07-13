---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fda.gov
  spf: true
hosts:
- cert_expires: Oct  2 18:57:13 2026 GMT
  host: open.fda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 11:20:53 2026 GMT
  host: api.fda.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Fda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for openFDA, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: openFDA
provider_slug: open-fda
slug: open-fda-domain-security
source_filename: open-fda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.fda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:57:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 11:20:53 2026 GMT\n  hsts: null\ndomains:\n- domain: fda.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-fda/refs/heads/main/security/open-fda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- FDA
- Food and Drug Administration
- Drug Safety
- Adverse Events
- Drug Labels
- Recalls
- Medical Devices
- Food Safety
- Tobacco
- Public Health
- Open Data
- Government
- Regulatory
- FAERS
- SPL
---
