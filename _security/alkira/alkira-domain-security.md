---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alkira.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: terraform.io
  spf: true
hosts:
- cert_expires: Sep 15 05:18:43 2026 GMT
  host: www.alkira.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: registry.terraform.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: your_tenant_name.portal.alkira.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''your_tenant'
kind: domain-security
layout: security
method: probed
name: Alkira Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alkira, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alkira
provider_slug: alkira
slug: alkira-domain-security
source_filename: alkira-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alkira.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:18:43 2026 GMT\n  hsts: null\n- host: registry.terraform.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your_tenant_name.portal.alkira.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''your_tenant'\n  hsts: null\ndomains:\n- domain: alkira.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: terraform.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alkira/refs/heads/main/security/alkira-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Networking
- Cloud
- Multi-Cloud
- Infrastructure
- Network as a Service
- SD-WAN
- Security
- Automation
---
