---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: micrographia.bio
  spf: false
hosts:
- host: micrographia.bio
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''micrographi'
kind: domain-security
layout: security
method: probed
name: Micrographia Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Micrographia Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Micrographia Bio
provider_slug: micrographia-bio
slug: micrographia-bio-domain-security
source_filename: micrographia-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: micrographia.bio\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''micrographi'\n  hsts: null\ndomains:\n- domain: micrographia.bio\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/micrographia-bio/refs/heads/main/security/micrographia-bio-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- Biotechnology
- Life Sciences
- Startup
---
