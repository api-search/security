---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: llmpress.org
  spf: true
hosts:
- host: llmpress.org
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''llmpress.or'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: llmpress-org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for llmpress-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: llmpress-org
provider_slug: llmpress-org
slug: llmpress-org-domain-security
source_filename: llmpress-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llmpress.org\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''llmpress.or'\n  hsts: null\ndomains:\n- domain: llmpress.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/llmpress-org/security/llmpress-org-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
---
