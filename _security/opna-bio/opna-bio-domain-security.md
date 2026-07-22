---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opnabio.com
  spf: true
hosts:
- host: opnabio.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''opnabio.com'
kind: domain-security
layout: security
method: probed
name: Opna Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opna Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Opna Bio
provider_slug: opna-bio
slug: opna-bio-domain-security
source_filename: opna-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opnabio.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''opnabio.com'\n  hsts: null\ndomains:\n- domain: opnabio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opna-bio/refs/heads/main/security/opna-bio-domain-security.yml
summary_line: DMARC
tags:
- Company
- Oncology
- Biopharmaceutical
- Pharmaceuticals
- Cancer
- Drug Discovery
- Life Sciences
- Healthcare
---
