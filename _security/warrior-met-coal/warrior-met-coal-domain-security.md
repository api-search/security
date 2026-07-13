---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: warriormetcoal.com
  spf: false
hosts:
- host: www.warriormetcoal.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.warrior'
- host: developer.warriormetcoal.com
  https: false
- host: api.warriormetcoal.com
  https: false
kind: domain-security
layout: security
method: probed
name: Warrior Met Coal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Warrior Met Coal, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Warrior Met Coal
provider_slug: warrior-met-coal
slug: warrior-met-coal-domain-security
source_filename: warrior-met-coal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.warriormetcoal.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.warrior'\n  hsts: null\n- host: developer.warriormetcoal.com\n  https: false\n- host: api.warriormetcoal.com\n  https: false\ndomains:\n- domain: warriormetcoal.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warrior-met-coal/refs/heads/main/security/warrior-met-coal-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Coal
- Mining
- Steel
---
