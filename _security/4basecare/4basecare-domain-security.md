---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 4basecare.com
  spf: true
hosts:
- cert_expires: Oct  7 10:31:59 2026 GMT
  host: www.4basecare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 08:14:48 2026 GMT
  host: galens.4basecare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 08:14:43 2026 GMT
  host: api.4basecare.com
  hsts: false
  https: true
  note: Private application backend for the Galens single-page app; not in apis.yml hosts so the probe script did not reach it. Probed by hand 2026-09-05 with the same openssl/HEAD method.
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 4Basecare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4baseCare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 4baseCare
provider_slug: 4basecare
slug: 4basecare-domain-security
source_filename: 4basecare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.4basecare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:31:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: galens.4basecare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 08:14:48 2026 GMT\n  hsts: false\n- host: api.4basecare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 08:14:43 2026 GMT\n  hsts: false\n  note: 'Private application backend for the Galens single-page app; not in apis.yml\n    hosts so the probe script did not reach it. Probed by hand 2026-09-05 with the\n    same openssl/HEAD method.'\ndomains:\n- domain: 4basecare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4basecare/refs/heads/main/security/4basecare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Precision Oncology
- Genomics
- Healthcare
- Cancer
- Diagnostics
- Artificial Intelligence
- Life Sciences
- Clinical Decision Support
- Next Generation Sequencing
- India
---
