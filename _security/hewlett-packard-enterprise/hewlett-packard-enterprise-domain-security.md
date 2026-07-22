---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hewlett-packard-enterprise.com
  spf: false
hosts:
- host: www.hewlett-packard-enterprise.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.hewlett'
kind: domain-security
layout: security
method: probed
name: Hewlett Packard Enterprise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hewlett-packard-enterprise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: hewlett-packard-enterprise
provider_slug: hewlett-packard-enterprise
slug: hewlett-packard-enterprise-domain-security
source_filename: hewlett-packard-enterprise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hewlett-packard-enterprise.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.hewlett'\n  hsts: null\ndomains:\n- domain: hewlett-packard-enterprise.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hewlett-packard-enterprise/refs/heads/main/security/hewlett-packard-enterprise-domain-security.yml
summary_line: DMARC
tags: []
---
