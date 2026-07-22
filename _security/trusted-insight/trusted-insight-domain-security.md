---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thetrustedinsight.com
  spf: true
hosts:
- host: thetrustedinsight.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''thetrustedi'
kind: domain-security
layout: security
method: probed
name: Trusted Insight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trusted Insight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trusted Insight
provider_slug: trusted-insight
slug: trusted-insight-domain-security
source_filename: trusted-insight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thetrustedinsight.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''thetrustedi'\n  hsts: null\ndomains:\n- domain: thetrustedinsight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trusted-insight/refs/heads/main/security/trusted-insight-domain-security.yml
summary_line: DMARC
tags:
- Company
---
