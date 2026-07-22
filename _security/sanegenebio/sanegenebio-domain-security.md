---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sanegenebio.com
  spf: true
hosts:
- host: sanegenebio.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''sanegenebio'
kind: domain-security
layout: security
method: probed
name: Sanegenebio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sanegenebio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: sanegenebio
provider_slug: sanegenebio
slug: sanegenebio-domain-security
source_filename: sanegenebio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sanegenebio.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''sanegenebio'\n  hsts: null\ndomains:\n- domain: sanegenebio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanegenebio/refs/heads/main/security/sanegenebio-domain-security.yml
summary_line: DMARC
tags:
- Company
- Biotechnology
- Genetic Medicine
- RNAi
- Therapeutics
- Metabolic Disease
- Drug Delivery
- Life Sciences
---
