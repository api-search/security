---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pipelineequity.com
  spf: true
hosts:
- host: pipelineequity.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''pipelineequ'
kind: domain-security
layout: security
method: probed
name: Pipeline Equity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pipeline Equity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pipeline Equity
provider_slug: pipeline-equity
slug: pipeline-equity-domain-security
source_filename: pipeline-equity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pipelineequity.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''pipelineequ'\n  hsts: null\ndomains:\n- domain: pipelineequity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pipeline-equity/refs/heads/main/security/pipeline-equity-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
